Задание 1. Создать Pod с именем hello-world
Создать манифест (yaml-конфигурацию) Pod.
Использовать image - gcr.io/kubernetes-e2e-test-images/echoserver:2.2.
Подключиться локально к Pod с помощью kubectl port-forward и вывести значение (curl или в браузере).

Решение:

<img width="278" alt="image" src="https://github.com/user-attachments/assets/2572cffc-b382-4e45-8416-7d958172fbd8">

<img width="548" alt="image" src="https://github.com/user-attachments/assets/1c19da2d-b893-473b-8398-86fe8091612d">



Задание 2. Создать Service и подключить его к Pod
Создать Pod с именем netology-web.
Использовать image — gcr.io/kubernetes-e2e-test-images/echoserver:2.2.
Создать Service с именем netology-svc и подключить к netology-web.
Подключиться локально к Service с помощью kubectl port-forward и вывести значение (curl или в браузере).
Решение:

<img width="434" alt="image" src="https://github.com/user-attachments/assets/a5348fa4-a578-4ae4-9625-adfc0f7d9f27">
<img width="288" alt="image" src="https://github.com/user-attachments/assets/0d80a353-1fec-4e55-b8aa-d86b95e518cd">
<img width="361" alt="image" src="https://github.com/user-attachments/assets/22156ca1-8ef4-44d6-a87d-3e39777b753f">

