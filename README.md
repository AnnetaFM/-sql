# Примеры запросов на языке SQL

## Таблицы:
Students:
- id – integer
- created_at – datetime
- name – string
- age – integer

## Courses:
- id – integer
- name – string
- created_at – datetime
- updated_at – datetime

## StudentCourses:
- id – integer
- student_id - integer
- course_id – integer
- grade - float

### Напишите запрос, который создаёт таблицу Students по приложенной схеме. ID - автоинкрементируемый ключ, ограничьте колонку age значениями от 0 до 200.

CREATE TABLE Students (
    Id INT AUTO_INCREMENT PRIMARY KEY,
    Created_at DATETIME,
    Name VARCHAR(255),
    Age INT CHECK (Age >= 0 AND Age <= 200)
);

### Напишите запрос, который создаёт таблицу Students по приложенной схеме. ID - автоинкрементируемый ключ, ограничьте колонку age значениями от 0 до 200.