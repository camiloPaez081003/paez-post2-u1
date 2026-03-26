# Análisis de Peticiones HTTP - Unidad 1

## Descripción

Repositorio de análisis de peticiones HTTP/HTTPS realizado con
Chrome DevTools y Postman como parte del laboratorio 2 de
Programación Web - Séptimo Semestre.

## Herramientas utilizadas

- Google Chrome + DevTools (panel Network)
- Postman (petición POST con tests)

## Análisis realizados

| #   | Tipo               | URL                                            | Código         |
| --- | ------------------ | ---------------------------------------------- | -------------- |
| 1   | GET HTML           | https://example.com                            | 200 OK / 304\* |
| 2   | GET JSON (exitoso) | https://jsonplaceholder.typicode.com/posts/1   | 200 OK         |
| 3   | GET JSON (fallido) | https://jsonplaceholder.typicode.com/posts/999 | 404 Not Found  |
| 4   | POST JSON          | https://jsonplaceholder.typicode.com/posts     | 201 Created    |

\* Nota: en algunos casos Chrome devuelve 304 Not Modified en lugar de 200 OK.

## Aprendizajes más relevantes

Durante este laboratorio se comprendió cómo inspeccionar peticiones HTTP y HTTPS reales, identificando métodos, códigos de estado y headers. Se observó la diferencia entre consumir páginas HTML y APIs REST (text/html vs application/json), así como la importancia de los códigos de estado (200, 404, 201). Además, se practicó el uso de Postman para simular una petición POST y validar automáticamente la respuesta con tests.

## Conclusiones

El análisis permitió afianzar la comprensión del ciclo de vida de las peticiones HTTP. Se evidenció cómo GET se utiliza para obtener información y POST para crear recursos, y cómo los códigos de estado comunican el resultado de cada operación. Las herramientas DevTools y Postman resultan esenciales para depurar aplicaciones y consumir APIs de manera eficiente.
