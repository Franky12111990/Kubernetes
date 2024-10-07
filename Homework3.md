Задание 1. Создать Deployment и обеспечить доступ к репликам приложения из другого Pod
Создать Deployment приложения, состоящего из двух контейнеров — nginx и multitool. Решить возникшую ошибку.
После запуска увеличить количество реплик работающего приложения до 2.
Продемонстрировать количество подов до и после масштабирования.
Создать Service, который обеспечит доступ до реплик приложений из п.1.
Создать отдельный Pod с приложением multitool и убедиться с помощью curl, что из пода есть доступ до приложений из п.1.

Решение:
манифест деплоймента:
```
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-multitool-deployment
spec:
  replicas: 1
  selector:
    matchLabels:
      app: nginx-multitool
  template:
    metadata:
      labels:
        app: nginx-multitool
    spec:
      containers:
      - name: nginx
        image: nginx
        ports:
        - containerPort: 80
      - name: multitool
        image: praqma/network-multitool
        ports:
        - containerPort: 8080
        env:
        - name: HTTP_PORT
          value: "8080"
        - name: HTTPS_PORT
          value: "8443"
```
<img width="515" alt="image" src="https://github.com/user-attachments/assets/00fca455-b09a-40af-a934-cda994519c50">

<img width="420" alt="image" src="https://github.com/user-attachments/assets/237f6f38-ca3c-4052-86ff-9724afc8638b">




Задание 2. Создать Deployment и обеспечить старт основного контейнера при выполнении условий
Создать Deployment приложения nginx и обеспечить старт контейнера только после того, как будет запущен сервис этого приложения.
Убедиться, что nginx не стартует. В качестве Init-контейнера взять busybox.
Создать и запустить Service. Убедиться, что Init запустился.
Продемонстрировать состояние пода до и после запуска сервиса.

```
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
spec:
  replicas: 1
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      initContainers:
      - name: init-container
        image: busybox
        command: ['sh', '-c', 'echo Init container running... && sleep 5']
      containers:
      - name: nginx
        image: nginx
        ports:
        - containerPort: 80
        lifecycle:
          postStart:
            exec:
              command: ["/bin/sh", "-c", "echo Starting NGINX..."]
```

<img width="832" alt="image" src="https://github.com/user-attachments/assets/d6cdea22-462f-405b-b009-3217c1912389">
