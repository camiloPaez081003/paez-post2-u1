# Análisis 3: Petición POST - API REST con Postman

## Configuración

- Método: POST
- URL: https://jsonplaceholder.typicode.com/posts
- Headers: Content-Type = application/json
- Body: JSON con campos title, body, userId

## Respuesta

- Código de estado: 201 Created
- Headers de respuesta: Content-Type, X-Powered-By, Location (si aparece)
- Cuerpo: objeto JSON enviado + campo id generado

## Tests

- Status 201 Created → OK
- Respuesta incluye id asignado → OK

## Diferencias entre GET y POST

- GET: solicita datos, no modifica el servidor.
- POST: envía datos para crear un recurso nuevo.
- GET devuelve 200/404, POST devuelve 201 cuando se crea exitosamente.

## Conclusión

La petición POST permitió crear un recurso en la API, confirmando la diferencia entre obtener información (GET) y enviar información (POST). Los tests en Postman validaron automáticamente que la respuesta fuera correcta.
