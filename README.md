Portal-frontend

**1) Формы, ajax**
- в случае успеха сервер ответ ok
- в случае ошибки сервер отвечает Fail

**2) Все ajax запросы обрабатываются только через *catch-API***

------------



-  **/catch/catch_registration** //Регистрация пользователя

**Ожидает получить POST :**
- **login** //str
- **password** //str
- **email** //str
- **phone** //str
- **type** *//если слушатель то '1', если лекционный центр то '2'*

---- **если type = 1 , так же ожидает получить POST:**
-  **full_name** //str format Ф.И.О.
-  **worker_position** //str - Должность
-  **worker_city** //str - город

---- **если type = 2 , так же ожидает получить POST:**
-  **full_name** //str
-  **inn** //int
-  **kpp** //int
-  **ogrn** //int
-  **jur_name** //str
-  **jur_address** //str
- **fiz_address** //str


------------



- **/catch/catch_login** //Логин пользователя в систему

**Ожидает получить POST:**

- **login** //str
- **password** //str


------------



- **/catch/catch_event** //Создание мироприятия

**Ожидает получить POST:**

- **event_name** //str
- **event_type** //int
- **event_way** //json
- **event_address** //str
- **event_start_time** //str format YYYY-mm-dd
- **event_end_time** //str format YYYY-mm-dd
- **lector_id** //id
- **event_photos** //json
- **event_description** //str
- **is_free** //bool(0/1)
- **price** //int
- **is_discount** //bool(0/1)
- **rule_point** //int
- **rule_sertificate** //bool(0/1)
- **event_main_img** //str


------------



- **/catch/catch_lector** //Создание нового лектора

**Ожидает получить POST:**

- **full_name** //str
- **worker_position** //str
- **phone** //int
- **email** //str
- **photo** //str
