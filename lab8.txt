create database lab7;

CREATE INDEX countries_name ON countries(name);
CREATE INDEX employees_name_surname ON employees(name,surname);
create index salary on employees(salary);
create index employees.substring on employees(substring(name from 1 for 4));
create index department_id on employees(department_id,salary);
create index budget on departments(department_id, budget);