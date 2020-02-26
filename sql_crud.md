# SQL Queries Básicas

Para esta tarea se utilizaron los elementos CRUD (Create, Read, Update and Delete).

## SELECT
De la base de datos, twitter.sql se trabajará con la tabla users, para saber cuales son los registros de la tabla ejecutamos el código:
```
SELECT * FROM users
```

## INSERT
El código utilizado para insertar el usuario Anton Lofer en la tabla de users fue el siguiente: 
```
INSERT INTO users (first_name, last_name, handle, birthday, created_at, updated_at)
VALUES ('Anton', 'Lofer', 'Real_T_Mac', '1993-05-21', NOW(), NOW())
```

## UPDATE
El usuario Anton ya no quería que su nombre fuese un apodo así se actualiza su primer nombre al de Antonio. El código utilizado se presenta a continuación:
```
UPDATE users SET first_name = 'Antonio'
WHERE id=6
```

## DELETE
Finalmente, el usuario Antonio Lofer desapareció del ciberespacio por lo que se debió eliminar su registro. El código es el siguiente:
```
DELETE FROM users
WHERE id =6
```