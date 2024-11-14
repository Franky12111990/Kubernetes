Задание 1. Создать Deployment приложения и решить возникшую проблему с помощью ConfigMap. Добавить веб-страницу
Создать Deployment приложения, состоящего из контейнеров nginx и multitool.
Решить возникшую проблему с помощью ConfigMap.
Продемонстрировать, что pod стартовал и оба конейнера работают.
Сделать простую веб-страницу и подключить её к Nginx с помощью ConfigMap. Подключить Service и показать вывод curl или в браузере.
Предоставить манифесты, а также скриншоты или вывод необходимых команд.

Решение:

<img width="130" alt="image" src="https://github.com/user-attachments/assets/584d1f9b-1c7f-48c6-8687-10d5acb09874">

<img width="341" alt="image" src="https://github.com/user-attachments/assets/cfeb6b52-366c-4355-a4e9-eb44ed4ba43b">

<img width="354" alt="image" src="https://github.com/user-attachments/assets/65a2dbf0-fbee-49a4-a532-6b86c5bf62c7">

<img width="682" alt="image" src="https://github.com/user-attachments/assets/de887466-e20f-44af-8a11-f5f8ecd760ea">


Задание 2. Создать приложение с вашей веб-страницей, доступной по HTTPS
Создать Deployment приложения, состоящего из Nginx.
Создать собственную веб-страницу и подключить её как ConfigMap к приложению.
Выпустить самоподписной сертификат SSL. Создать Secret для использования сертификата.
Создать Ingress и необходимый Service, подключить к нему SSL в вид. Продемонстировать доступ к приложению по HTTPS.
Предоставить манифесты, а также скриншоты или вывод необходимых команд.

Решение:

<img width="485" alt="image" src="https://github.com/user-attachments/assets/ab3b269a-1006-4cf7-84c3-08a5a771a976">
<img width="404" alt="image" src="https://github.com/user-attachments/assets/7e0bce51-77fc-44cf-86f2-52bea9cb012c">
<img width="174" alt="image" src="https://github.com/user-attachments/assets/478bad9e-0ca6-479f-a034-327687640103">
<img width="208" alt="image" src="https://github.com/user-attachments/assets/901f9db4-91dd-4f94-831d-460062bec116">




