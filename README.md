# Task8
1. Создать инстанс для базы данных типа postgres с именем cluster_jun. <br>


![image](https://github.com/user-attachments/assets/0605a320-222c-4022-9662-c031f6ff5f82)
_________________________________________________________________________________________
2. Подключится к ней через pgAdmin установленный на ПК и через командную строке терминала линукс через терминальный клиент psql. <br>


![image](https://github.com/user-attachments/assets/aa1594fd-46f7-4556-b5b2-32ecb970443f) <br>
![image](https://github.com/user-attachments/assets/f863019a-18e9-48b0-a806-bf148c578c92)
_________________________________________________________________________________________
3. Cоздать в кластере баз данных postgres базу данных jun_db. <br>


![image](https://github.com/user-attachments/assets/d6bc73cc-1770-4013-ae48-38b1a46b989a) <br>
![image](https://github.com/user-attachments/assets/09f503b9-db59-4952-b74d-8f5eb952c331)
_________________________________________________________________________________________
4. Создать в ней таблицу под названием credit_cards_numbers. <br>


![image](https://github.com/user-attachments/assets/40f97e8e-578f-4a31-a14d-65766d3054c1) <br>
![image](https://github.com/user-attachments/assets/18887902-0120-4c68-a0de-dfa77a860d07) <br>
_________________________________________________________________________________________
5. Руками сделать snapshot. Удалить базу данных. Восстановить её из snapshots. Проверить наличие созданной таблицы через pgAdmin и терминальный клиент psql. <br>


Создание snapshot: <br>
![image](https://github.com/user-attachments/assets/f7f9c287-450f-4932-9779-ad5df584d306) <br>

Удаление базы - ``` postgres=> DROP DATABASE jun_db; ``` <br>
![image](https://github.com/user-attachments/assets/00741a78-83f2-4bf8-9aac-6f5f1009f885) <br>

Восстановление: <br>
![image](https://github.com/user-attachments/assets/9c0a5821-54f3-4e20-85e2-bb2ea42741b9) <br>

ИТОГ: <br>
![image](https://github.com/user-attachments/assets/234f441a-b72d-4a4f-b35b-17941e97392b) <br>
![image](https://github.com/user-attachments/assets/858a76a4-6652-40ca-920f-3cf22c92fe8e) <br>
__________________________________________________________________________________________
6. Настроить её бэкапы через AWS Backup по расписанию раз в час например. <br>
Создал vault: <br>
![image](https://github.com/user-attachments/assets/99175c56-80ce-42f7-b3e7-f1d58add166d) <br>

Создал план и Resource assignment: <br>
![image](https://github.com/user-attachments/assets/c1b174cf-20bd-480d-98c0-16fd383b0f0b) <br>

![image](https://github.com/user-attachments/assets/4b91516c-b27b-48c3-a990-1ed91204f267) <br>

После добавил TAG на базу данных

Дождался backup job: <br>
![image](https://github.com/user-attachments/assets/af4e8506-c62c-4bde-98c8-9e4ad08f364e) <br>

Удалил базу данных и восстановил: <br>
![image](https://github.com/user-attachments/assets/e8f9489a-bb90-4335-87a0-287851156fc3) <br>


![image](https://github.com/user-attachments/assets/193606a4-a4cc-48d3-b1e7-cd63a910a14a) <br>

![image](https://github.com/user-attachments/assets/2fe7c2d0-6366-4a3b-8d2e-476aec4c81be)











