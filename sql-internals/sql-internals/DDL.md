- Data Definition Languauge : This is nothing but the creation of object's body to store data such as CREATE a table, ALTER, DROP.

- DDL is more like a creation of a container to store data in structured formate, hence we define the format.

- Create is used to create objects (with schema and without data eyt)

- An object is a real world's entity such as person, car, chair, weather, employee, department (Something that exists in real world)

CREATE TABLE person(
id INT NOT NULL,
name VARCHAR(50) NOT NULL,
phone VARCHAR(50) NOT NULL,
DOB DATE,
CONSTRAINT id_pk PRIMARY KEY(id)
);

- ALTER is used to alter the table's definition or body

ALTER TABLE person(
    ADD email VARCHAR(20)
) //Always added to end of the table

ALTER TABLE person(
    MODIFY COLUMN email VARCHAR(50)
)

ALTER TABLE person(
    DROP COLUMN email
) // No need to mention data type here as DBMS already knows it.

DROP - delete the entire object with data (Nothing will exist)

DROP TABLE person; (Dangerous command)


-- DDL is basically used to create the body/structure for the objects we want to create.

-- When you want to alter a table's structure, may be have the column DOB at the start, then we cannot change the position of it. We will have to drop the table and create a new one. Because once create, we can just alter or modify related to datatype or column name, the position will be fixed and we will have to create a new one if we want, by dropping the old one.


