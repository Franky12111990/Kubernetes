Задание 1. Создать Deployment и обеспечить доступ к контейнерам приложения по разным портам из другого Pod внутри кластера
Создать Deployment приложения, состоящего из двух контейнеров (nginx и multitool), с количеством реплик 3 шт.
Создать Service, который обеспечит доступ внутри кластера до контейнеров приложения из п.1 по порту 9001 — nginx 80, по 9002 — multitool 8080.
Создать отдельный Pod с приложением multitool и убедиться с помощью curl, что из пода есть доступ до приложения из п.1 по разным портам в разные контейнеры.
Продемонстрировать доступ с помощью curl по доменному имени сервиса.
Предоставить манифесты Deployment и Service в решении, а также скриншоты или вывод команды п.4.

Решение:

<img width="515" alt="image" src="https://github.com/user-attachments/assets/4e5e0441-3052-4675-b464-3baeb9c9f3b5">

<img width="472" alt="image" src="https://github.com/user-attachments/assets/5951c647-4321-4944-af04-53e1c5c8b39e">

<img width="722" alt="image" src="https://github.com/user-attachments/assets/55613709-d61d-457d-8ee1-d63f879b9161">

<img width="949" alt="image" src="https://github.com/user-attachments/assets/eef252d3-6597-4591-80ea-d440a6fceccc">



Задание 2. Создать Service и обеспечить доступ к приложениям снаружи кластера
Создать отдельный Service приложения из Задания 1 с возможностью доступа снаружи кластера к nginx, используя тип NodePort.
Продемонстрировать доступ с помощью браузера или curl с локального компьютера.
Предоставить манифест и Service в решении, а также скриншоты или вывод команды п.2.

Решение:

<img width="482" alt="image" src="https://github.com/user-attachments/assets/0ba22b11-e784-4e11-9c53-7be44bf09941">

<img width="554" alt="image" src="https://github.com/user-attachments/assets/54ccf8a2-893a-4a0f-ab89-d410b403666f">

