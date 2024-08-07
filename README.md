# ProContactoPruebaPractica
Evaluación práctica de reclutamiento para la empresa ProContacto

¿Qué te motivó a elegir tu carrera profesional? 

Los diferentes campos de aplicación, la variedad de trabajo que puede haber y las diferentes modalidades, que es algo internacional 

¿Qué esperas aprender o lograr en este nuevo rol? 

Espero mejorar mis habilidades como  

¿Cómo te mantenes actualizado en tu campo profesional? 

Escuchando activamente a diferentes colegas y leyendo noticias tecnológicas 

¿Qué valores personales consideras importantes en el ámbito laboral? 

Responsabilidad, proactividad, manejo del tiempo, respeto y amabilidad 


# Ejercicio 2: Comprensión del Protocolo HTTP

Las siguientes preguntas están orientadas a la comprensión del protocolo HTTP. Son agnósticas al lenguaje de programación, la idea es comprender los conceptos del estándar.

## 1. ¿Qué es un servidor HTTP?

Un servidor HTTP es un software que comprende y responde a las solicitudes HTTP de los clientes (normalmente navegadores web). Maneja solicitudes entrantes, procesa las solicitudes y devuelve las respuestas apropiadas al cliente, como páginas web, imágenes, videos u otros recursos.

## 2. ¿Qué son los verbos HTTP? Mencionar los más conocidos

Los verbos HTTP, también conocidos como métodos HTTP, son acciones que los clientes pueden solicitar que realice el servidor. Los más conocidos son:

- **GET**: Solicita un recurso del servidor.
- **POST**: Envía datos al servidor para ser procesados.
- **PUT**: Actualiza un recurso existente o crea uno nuevo si no existe.
- **DELETE**: Elimina un recurso del servidor.
- **PATCH**: Aplica modificaciones parciales a un recurso.
- **HEAD**: Similar a GET, pero solo solicita los headers de la respuesta.
- **OPTIONS**: Describe las opciones de comunicación para el recurso de destino.

## 3. ¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?

- **Request**: Es una solicitud enviada por un cliente al servidor. Contiene una línea de solicitud, headers y, opcionalmente, un cuerpo de mensaje.
- **Response**: Es la respuesta enviada por el servidor al cliente. Contiene una línea de estado, headers y, opcionalmente, un cuerpo de mensaje.
- **Headers**: Son pares clave-valor incluidos en las solicitudes y respuestas HTTP que transmiten información adicional sobre la solicitud o respuesta. Ejemplos incluyen `Content-Type`, `Authorization`, `User-Agent`, etc.

## 4. ¿Qué es un queryString? (En el contexto de una URL)

Un queryString es una parte de la URL que se utiliza para pasar parámetros a una página web. Comienza con un signo de interrogación (?) y consiste en pares clave-valor separados por &. Por ejemplo: `http://example.com/page?name=John&age=30`.

## 5. ¿Qué es el responseCode? ¿Qué significado tienen los posibles valores devueltos?

El responseCode es un código de estado en la respuesta HTTP que indica el resultado de la solicitud. Algunos códigos comunes son:

- **1xx (Informational)**: Indica que la solicitud fue recibida y el proceso continúa.
- **2xx (Success)**: Indica que la solicitud fue recibida, entendida y aceptada con éxito.
  - **200 OK**: Solicitud exitosa.
  - **201 Created**: Recurso creado exitosamente.
- **3xx (Redirection)**: Indica que se requieren acciones adicionales para completar la solicitud.
  - **301 Moved Permanently**: El recurso fue movido permanentemente a una nueva URL.
  - **302 Found**: El recurso fue encontrado en una URL diferente.
- **4xx (Client Error)**: Indica errores del cliente.
  - **400 Bad Request**: Solicitud malformada.
  - **401 Unauthorized**: Autenticación requerida.
  - **404 Not Found**: Recurso no encontrado.
- **5xx (Server Error)**: Indica errores del servidor.
  - **500 Internal Server Error**: Error general del servidor.
  - **503 Service Unavailable**: Servicio no disponible.

## 6. ¿Cómo se envía la data en un GET y cómo en un POST?

- **GET**: La data se envía en la URL como parte del queryString. Ejemplo: `http://example.com/page?name=John&age=30`.
- **POST**: La data se envía en el cuerpo de la solicitud. No es visible en la URL.

## 7. ¿Qué verbo HTTP utiliza el navegador cuando accedemos a una página?

El navegador utiliza el verbo **GET** cuando accedemos a una página web.

## 8. Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.

**JSON (JavaScript Object Notation)**: Es un formato de datos ligero y fácil de leer/escribir para humanos y máquinas. Utiliza pares clave-valor y listas ordenadas.
```json
{
  "name": "John",
  "age": 30,
  "children": ["Anna", "Billy"]
}
```

XML (eXtensible Markup Language): Es un formato de datos más rígido que JSON, utilizado para almacenar y transportar datos. Usa etiquetas para definir elementos.

```xml
<person>
  <name>John</name>
  <age>30</age>
  <children>
    <child>Anna</child>
    <child>Billy</child>
  </children>
</person>
```


## 9. Explicar brevemente el estándar SOAP
SOAP (Simple Object Access Protocol) es un protocolo de comunicación que utiliza XML para estructurar mensajes y permite la comunicación entre aplicaciones a través de redes, especialmente en servicios web. Es independiente del lenguaje de programación y puede funcionar sobre varios protocolos de transporte como HTTP, SMTP, etc.

## 10. Explicar brevemente el estándar RESTful
REST (Representational State Transfer) es un estilo arquitectónico para servicios web que utiliza HTTP y se basa en operaciones sin estado, identificadores de recursos (URLs) y una comunicación clara a través de métodos HTTP estándar (GET, POST, PUT, DELETE). RESTful describe servicios web que siguen los principios REST.

## 11. ¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?
Los headers en un request son pares clave-valor que proporcionan información adicional sobre la solicitud, como el tipo de contenido, autenticación, longitud del contenido, etc. El key Content-Type se utiliza para especificar el tipo de contenido del cuerpo de la solicitud o respuesta, por ejemplo, application/json para JSON, text/html para HTML, etc.


