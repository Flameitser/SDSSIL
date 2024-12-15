# SDSSIL
Системы сбора событий и логов.

ББМО-02-23 Курченко И.Д.

## Практика № 4 Network Threat Hunting

# Скачиваем и разворачиваем образ.

![image](https://github.com/user-attachments/assets/c93d35b2-5028-4605-b2c4-48c1bc10191c)

Вход в систему по паролю hunting

![image](https://github.com/user-attachments/assets/2d362c22-5b8c-46fe-add9-444f28cbc229)

Логин и пароль для входа в веб-версию:

 Name: threat@activecountermeasures.com
 
 Pass: hunting2


![image](https://github.com/user-attachments/assets/fe58db63-72d6-44de-95c9-4e4c74dc38a3)

![image](https://github.com/user-attachments/assets/954addbe-f311-4d3b-9559-109ec6743f1c)

![image](https://github.com/user-attachments/assets/c2811983-ea00-43c5-8b9b-e9a00ea3b489)

![image](https://github.com/user-attachments/assets/a0360c14-b053-430c-8574-7a5c0252e92c)

![image](https://github.com/user-attachments/assets/5831d4af-a9f3-4225-9c51-44ef50b56c4b)


Импортируем логи

![image](https://github.com/user-attachments/assets/7f0527ef-fd2b-4043-9eb3-0ac3db52404d)

![image](https://github.com/user-attachments/assets/32a0067c-12c8-421e-9879-0c8787134699)

![image](https://github.com/user-attachments/assets/d4164376-1cbe-42df-81ae-c637b898adb1)

![image](https://github.com/user-attachments/assets/56ac8d08-621d-4309-8287-78b043426ea8)

Анализ всех адресов выявил следующее:

Высокий уровень согласованности метрик (99.70%)

Такой высокий уровень согласованности (кумулятивная метрика соответствия) может указывать на регулярные и четко организованные запросы от источника к целевому IP-адресу. Это может быть признаком Beaconing-а, когда зараженное устройство устанавливает связь с управляющим сервером (C2).

Общее количество соединений (3011)
Для одного IP-адреса это значительное количество соединений. Если такая активность характерна для сети, это может не быть аномалией. Однако, если подобная активность не ожидается (например, для обычного пользователя или устройства IoT), это может свидетельствовать о нежелательном поведении.
Равномерное распределение активности на графике

Использование HTTP без шифрования
Отсутствие HTTPS может указывать на то, что данные передаются в незашифрованном виде, что создает риски. Незащищенные протоколы часто используются для связи с C2-серверами.

Заключение
Практически все адреса связаны с Windows, поэтому мы добавляем их в белый список.
