# Домашнее задание "Базы данных" - Зябликова Анастасия

# Задание 1

CREATE TABLE employee (
   employee_id int,
   employee_name varchar(50) NOT NULL,
   employee_salary mediumint,
   employee_position varchar(50) NOT NULL,
   employee_hiring_date date
   employee_project text[]
);

CREATE TABLE divison_type (
   division_id int
   division_name varchar(50)
);
 
CREATE TABLE structural_division (
   structural_division_id int,
   structural_division_name varchar(50) NOT NULL,
   division_address varchar(50),
   division_type_id int
);

CREATE TABLE division_address (
   division_address_id int,
   division_address_name varchar(255)
);

CREATE TABLE project (
   project_id int
   project_name varchar(255)
   employee_id int
);


CREATE TABLE position (
   position_id int
   position_name varchar (50)
   structural_division_id int
);

CREATE TABLE division_project (
  structural_division_id int,
  project_name varchar(255)
);
