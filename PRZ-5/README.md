# SDSSIL
Системы сбора событий и логов.

ББМО-02-23 Курченко И.Д.

## Практика № 5 Network Threat Hunting


## 1. Скачивание образа
Для начала скачиваем образ ubunta по ссылке https://ubuntu.com/download/desktop

![image](https://github.com/user-attachments/assets/c57c6619-d37c-48eb-8f19-2320e9fcbbb0)


## 2. Установка 2-ух образов

![image](https://github.com/user-attachments/assets/bef205cb-33bd-40a2-8084-361d691978b1)



## 3. Проверка сетевой связности

![image](https://github.com/user-attachments/assets/135a98b7-a5b0-42b8-9bd5-a2a430cee19c)


![image](https://github.com/user-attachments/assets/2aa91d47-51e1-4d57-906d-adab3f912602)



## 4. Установка Wazuh

Заходим под рутом и вводим команду " curl -sO htt://packages.wazuh.com/4.7/wazuh-install.sh && sudo bash ./wazuh-install.sh -a " для установки
Так же нужно добавить флаг -i, чтобы убрать предупреждение

![image](https://github.com/user-attachments/assets/7bab5869-4dd0-4978-9e88-e8e5866b90cb)

После установки перейдем по ссылке "https://localhost/app/wazuh" для входа в веб-версию

Логин и пароль для входа ниже

![image](https://github.com/user-attachments/assets/4a2b70ea-bf00-427b-a09a-46a245a1fe8e)

![image](https://github.com/user-attachments/assets/c78e8504-865f-413d-a586-77ec61f6c166)

Нажимаем add agent

![image](https://github.com/user-attachments/assets/ddaad55d-6783-4f7e-a689-a5c2ec750833)

![image](https://github.com/user-attachments/assets/a326c574-1d5b-4e77-93ac-9056f0734025)

![image](https://github.com/user-attachments/assets/615f4094-6f73-4247-9c9b-d5a672c53a25)


![image](https://github.com/user-attachments/assets/6c49d0c7-c0f0-4d18-a851-36127347a150)

![image](https://github.com/user-attachments/assets/6f66f738-8001-4b47-86d4-1e947132193f)

## 5. Установленный агент

![image](https://github.com/user-attachments/assets/b90c15db-5dc0-46df-8f19-9a637bf39fce)


## 6. Скачиваем Suricata на клиентскую ВМ

![image](https://github.com/user-attachments/assets/f6a412ca-dfc7-42c5-902d-4159089b7282)

![image](https://github.com/user-attachments/assets/5bf26f17-3be2-4582-a67d-423b59775058)

## 7. Кофинг Suricata 

![image](https://github.com/user-attachments/assets/27401bd8-ee8f-4669-8390-8615e3b3aa98)

![image](https://github.com/user-attachments/assets/96cf3118-7470-4622-a061-3829a4151b29)

![image](https://github.com/user-attachments/assets/5044ec32-969e-42bc-96b0-343a59724fb9)

![image](https://github.com/user-attachments/assets/3b4b45a8-7517-4597-abe8-01cc20670b88)


## 8. Логи Suricata

![image](https://github.com/user-attachments/assets/aa1812ea-7839-4426-8e31-02e0ae229fc7)

![image](https://github.com/user-attachments/assets/6900f14e-2929-4820-beb2-64cf943fdc9d)

## 9. Провеерка Suricata

На ВМ Kali выполним ping клиентскую ВМ, проверка наличия обнаружения активности

![image](https://github.com/user-attachments/assets/4e541aa1-3de1-4c4c-b987-7a613cf299a0)

![image](https://github.com/user-attachments/assets/b2c1fb15-c8f6-4030-b6f8-68b5e0f62937)


## 10. Установка Yara на клиентскую ВМ

![image](https://github.com/user-attachments/assets/8c7be745-0a66-409d-9779-90e93f3441d3)

## 11. Скрипт yara.sh для получения данных в Wazuh

![image](https://github.com/user-attachments/assets/9f330858-3832-4ece-8c85-cadd95d53574)

## 12. Настройка Серверной ВМ для работы с YARA

![image](https://github.com/user-attachments/assets/6729b9c9-8bc1-4cee-b0b6-bf2e115f8419)

![image](https://github.com/user-attachments/assets/eca1699d-d7e8-4d51-a0b3-480d76a71e5c)

