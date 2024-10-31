Задание 1
Что нужно сделать

Создать Deployment приложения, состоящего из двух контейнеров и обменивающихся данными.

Создать Deployment приложения, состоящего из контейнеров busybox и multitool.
Сделать так, чтобы busybox писал каждые пять секунд в некий файл в общей директории.
Обеспечить возможность чтения файла контейнером multitool.
Продемонстрировать, что multitool может читать файл, который периодоически обновляется.
Предоставить манифесты Deployment в решении, а также скриншоты или вывод команды из п. 4.

Решение:

<img width="644" alt="image" src="https://github.com/user-attachments/assets/48c8ae93-907c-4ac2-9326-6a90a8edd1d0">



Задание 2
Что нужно сделать

Создать DaemonSet приложения, которое может прочитать логи ноды.

Создать DaemonSet приложения, состоящего из multitool.
Обеспечить возможность чтения файла /var/log/syslog кластера MicroK8S.
Продемонстрировать возможность чтения файла изнутри пода.
Предоставить манифесты Deployment, а также скриншоты или вывод команды из п. 2.

Решение:
<img width="331" alt="image" src="https://github.com/user-attachments/assets/363dbb88-e907-4a13-8a3f-61ab0d846bcd">


<img width="454" alt="image" src="https://github.com/user-attachments/assets/1d3b704e-e9ba-49d3-83d6-07b1f8275137">

<img width="798" alt="image" src="https://github.com/user-attachments/assets/82f398a3-c4c0-40cf-a875-e9e775b2a169">


<img width="877" alt="image" src="https://github.com/user-attachments/assets/4e2de87d-71a4-4495-84b7-e29540b226c9">

