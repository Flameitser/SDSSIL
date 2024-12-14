# SDSSIL
Системы сбора событий и логов.

ББМО-02-23 Курченко И.Д.

Практика № 3


## 1. Скачивание образа
Для начала скачивыаем обрпз убунты по ссылке https://ubuntu.com/download/desktop

![image](https://github.com/user-attachments/assets/c57c6619-d37c-48eb-8f19-2320e9fcbbb0)


## 2. Установка образа

![image](https://github.com/user-attachments/assets/bef205cb-33bd-40a2-8084-361d691978b1)



## 3. Проверка сетевой связности

![image](https://github.com/user-attachments/assets/135a98b7-a5b0-42b8-9bd5-a2a430cee19c)


![image](https://github.com/user-attachments/assets/2aa91d47-51e1-4d57-906d-adab3f912602)


## 4. Проверка видимости друг-друга

![image](https://github.com/user-attachments/assets/8856d1f2-5ea0-4242-a95e-5f1d9ce15d4a)




## 5. Установка Wazuh

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

Установленный агент

![image](https://github.com/user-attachments/assets/b90c15db-5dc0-46df-8f19-9a637bf39fce)

![image](https://github.com/user-attachments/assets/f8bdfd94-5763-4b9a-8792-af8f03c2ec20)


## Выявление уязвимостей

Внесенные в файл ossec.conf изменения
![image](https://github.com/user-attachments/assets/7325af33-2c44-4f47-a604-f8531dc2caf2)

Выявление уязвимостей пакетов на клиенте ("агенте")

![image](https://github.com/user-attachments/assets/81068543-0982-4db6-bd44-42fae77ac486)

Просмотр логов

![image](https://github.com/user-attachments/assets/fc216ef6-e4c6-4b47-ae61-efb6c692053d)

![image](https://github.com/user-attachments/assets/d68aac14-bb0b-4f8f-910b-36cda94624a0)

![image](https://github.com/user-attachments/assets/f5f29624-292d-4dcb-b572-cad71e683045)

![image](https://github.com/user-attachments/assets/e2686439-eb4d-44d7-ac01-cffbaadaf236)

![image](https://github.com/user-attachments/assets/30374306-b7cc-4538-bd02-02f47711626b)

![image](https://github.com/user-attachments/assets/46b97794-46e5-4e8a-bf53-b419c230f797)



