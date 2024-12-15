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


## 6. Скачиваем Suricata

![image](https://github.com/user-attachments/assets/f6a412ca-dfc7-42c5-902d-4159089b7282)

![image](https://github.com/user-attachments/assets/5bf26f17-3be2-4582-a67d-423b59775058)

## 7. Кофинг Suricata 

![image](https://github.com/user-attachments/assets/27401bd8-ee8f-4669-8390-8615e3b3aa98)

![image](https://github.com/user-attachments/assets/96cf3118-7470-4622-a061-3829a4151b29)

![image](https://github.com/user-attachments/assets/5044ec32-969e-42bc-96b0-343a59724fb9)

