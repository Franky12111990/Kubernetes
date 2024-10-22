Задание 1. Создать Deployment приложений backend и frontend
Создать Deployment приложения frontend из образа nginx с количеством реплик 3 шт.
Создать Deployment приложения backend из образа multitool.
Добавить Service, которые обеспечат доступ к обоим приложениям внутри кластера.
Продемонстрировать, что приложения видят друг друга с помощью Service.
Предоставить манифесты Deployment и Service в решении, а также скриншоты или вывод команды п.4.

Решение:

<img width="920" alt="image" src="https://github.com/user-attachments/assets/c7978a92-89ea-4d74-adb2-9b8961067524">

<img width="278" alt="image" src="https://github.com/user-attachments/assets/2c3f565d-516f-4bfc-b5a8-080e2879a665">

<img width="443" alt="image" src="https://github.com/user-attachments/assets/f3966d5e-86ac-4bf7-8caa-ef801a8a3620">

<img width="215" alt="image" src="https://github.com/user-attachments/assets/bfa4745d-4be5-4f53-af98-b67ea422cc49">

<img width="247" alt="image" src="https://github.com/user-attachments/assets/93080dbb-127f-4648-80fb-2df78b2fe962">







Задание 2. Создать Ingress и обеспечить доступ к приложениям снаружи кластера
Включить Ingress-controller в MicroK8S.
Создать Ingress, обеспечивающий доступ снаружи по IP-адресу кластера MicroK8S так, чтобы при запросе только по адресу открывался frontend а при добавлении /api - backend.
Продемонстрировать доступ с помощью браузера или curl с локального компьютера.
Предоставить манифесты и скриншоты или вывод команды п.2.

<img width="377" alt="image" src="https://github.com/user-attachments/assets/d07ed542-d24e-4c95-95f3-539ce7d34477">

<img width="321" alt="image" src="https://github.com/user-attachments/assets/7653fa05-44a8-44f7-8ea2-36d7feed2be7">


