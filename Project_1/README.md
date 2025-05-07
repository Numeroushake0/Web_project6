# Project 1 — Student Database

# Опис
Цей проєкт створює базу даних студентів, заповнює її випадковими даними за допомогою Faker та дозволяє виконувати SQL-запити для аналітики.

# Кроки запуску
1. Створіть базу даних у PostgreSQL (наприклад, `your_db`).
2. Виконайте SQL-скрипт для створення таблиць:
    ```
    psql -U your_user -d your_db -f characteristics/create_tables.sql
    ```
3. Встановіть залежності:
    ```
    pip install -r requirements.txt
    ```
4. Заповніть базу даних:
    ```
    python data_generation/populate_db.py
    ```
5. Запити знаходяться в `characteristics/queries/`. Їх можна виконувати у SQL-клієнті або через Python.

# Структура
- `characteristics/create_tables.sql` — створення таблиць
- `data_generation/populate_db.py` — генерація та заповнення даних
- `characteristics/queries/` — SQL-запити
