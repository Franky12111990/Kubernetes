Задание 1
Что нужно сделать

Создать Deployment приложения, использующего локальный PV, созданный вручную.

Создать Deployment приложения, состоящего из контейнеров busybox и multitool.
Создать PV и PVC для подключения папки на локальной ноде, которая будет использована в поде.
Продемонстрировать, что multitool может читать файл, в который busybox пишет каждые пять секунд в общей директории.
Удалить Deployment и PVC. Продемонстрировать, что после этого произошло с PV. Пояснить, почему.
Продемонстрировать, что файл сохранился на локальном диске ноды. Удалить PV. Продемонстрировать что произошло с файлом после удаления PV. Пояснить, почему.
Предоставить манифесты, а также скриншоты или вывод необходимых команд.

Решение:


<img width="665" alt="image" src="https://github.com/user-attachments/assets/ed870350-a43d-445b-90be-87174a9b2580">
<img width="674" alt="image" src="https://github.com/user-attachments/assets/534fef62-2f68-41d0-a717-2dda248ee082">

PV не будет удален из-за настроенной политики Retain

<img width="276" alt="image" src="https://github.com/user-attachments/assets/aaceff03-ee5a-455f-a46a-55a184431fc3">


<img width="261" alt="image" src="https://github.com/user-attachments/assets/f64a796f-6406-4819-a18c-1c25c3df9ba4">

<img width="163" alt="image" src="https://github.com/user-attachments/assets/f87f9762-23ec-4aa1-b568-dc6fd2cbeef8">

<img width="533" alt="image" src="https://github.com/user-attachments/assets/92b0efef-fdee-4d76-8515-4040c3434b30">

<img width="563" alt="image" src="https://github.com/user-attachments/assets/9360e882-d2fa-4c0f-8f33-7a355ccfaea0">

Задание 2
Что нужно сделать

Создать Deployment приложения, которое может хранить файлы на NFS с динамическим созданием PV.

Включить и настроить NFS-сервер на MicroK8S.
Создать Deployment приложения состоящего из multitool, и подключить к нему PV, созданный автоматически на сервере NFS.
Продемонстрировать возможность чтения и записи файла изнутри пода.
Предоставить манифесты, а также скриншоты или вывод необходимых команд.

Решение:

<img width="514" alt="image" src="https://github.com/user-attachments/assets/93da439a-ebc2-45f0-9aa0-0b671bf41d6f">

<img width="314" alt="image" src="https://github.com/user-attachments/assets/2db27e9c-2fb1-4b99-9841-14efe9babd6c">


<img width="202" alt="image" src="https://github.com/user-attachments/assets/7ddb710b-b3e7-4203-bc2a-dfb26c9d32bb">

<img width="220" alt="image" src="https://github.com/user-attachments/assets/a195d7a8-7106-4b4b-a069-4061636e1911">

<img width="524" alt="image" src="https://github.com/user-attachments/assets/ff0bf8ef-6e42-4497-84d6-6f9b5cfe34aa">




