# Análisis 2: Petición GET - API REST

## Información general

- URL: https://jsonplaceholder.typicode.com/posts/1
- Método: GET
- Código de estado: 304 OK

## Headers de Request

| Header     | Valor                        |
| ---------- | ---------------------------- |
| Host       | jsonplaceholder.typicode.com |
| User-Agent | [tu navegador]               |
| Accept     | application/json             |

## Headers de Response

| Header        | Valor            | Significado                                  |
| ------------- | ---------------- | -------------------------------------------- |
| Content-Type  | application/json | Indica que la respuesta está en formato JSON |
| Cache-Control | [valor]          | Control de caché                             |
| Date          | [valor]          | Fecha de la respuesta                        |

## Comparación HTML vs API REST

- La petición HTML (example.com) devolvía `Content-Type: text/html`.
- La petición API REST devuelve `Content-Type: application/json`.
- En HTML recibimos un documento renderizable, mientras que en API REST recibimos datos estructurados.

## Petición fallida

- URL: https://jsonplaceholder.typicode.com/posts/999
- Método: GET
- Código de estado: 404 Not Found

## Conclusión

En este análisis se observa cómo una API REST responde con datos JSON en una petición exitosa (304) y con un error controlado (404 Not Found) cuando el recurso no existe. Esto demuestra la diferencia entre consumir páginas HTML y consumir APIs.
