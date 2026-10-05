# Documentación para personal de la empresa
Una introducción a la plataforma coT4, qué es, su creación y funcionamiento.

### ¿Qué es la plataforma coT4? 

<p align="justify">
   Cotizador en línea comercial diseñado para optimizar el proceso de venta y atención al cliente, una cotización inmediata que transforma rápidamente la solicitud del cliente en un ticket de compra a través de su correo electrónico.
</p>

<p align="justify">
La plataforma permite optimizar el flujo de información entre el cliente y las áreas involucradas en el proceso de cotización, reduciendo errores en la captura de datos, agilizando la revisión de las solicitudes y facilitando el seguimiento de cada requerimiento hasta la generación y envío de la cotización correspondiente.
</p>

<p align="justify">
Para su correcto funcionamiento, es necesario que la información ingresada por parte del usuario en el formato sea completa y precisa, ya que los datos proporcionados constituyen la base para el procesamiento y cálculo de la cotización por la plataforma.
</p>

**Impacto Operativo:**

<ul style="text-align: justify;">
  <li>Automatiza la generación de correos con la cotización lista, reduciendo la carga operativa del equipo de ventas y los tiempos de respuesta para el cliente</li>
  <li>Garantiza la captura precisa de la información del cliente y del producto solicitado a través de campos obligatorios y filtros configurados en el formato cotizador</li>
  <li>Permite capturar y procesar cotizaciones en cualquier momento aumentando la capacidad de atención de la empresa</li>
</ul>

<p align="justify">

---

### ¿Cómo funciona la plataforma?

<p align="justify">
La plataforma opera como un flujo de trabajo digital automático que procesa solicitudes de cotización desde la captura inicial de datos por parte del usuario hasta el procesamiento completo.
</p>

**1. Captura e Ingreso de Datos**
<p align="justify">
El proceso inicia cuando el cliente descarga la plantilla del formato cotizador e ingresa la información requerida (datos del solicitante, envío, facturación y especificaciones técnicas del producto solicitado) mediante campos de texto manuales y menús desplegables. Una vez completado, el archivo es cargado en la plataforma para su procesamiento.
</p>

**2. Procesamiento de la Interfaz y Validación**
<p align="justify">
Al enviar el formulario, el sistema ajusta dinámicamente el estado del proceso a ejecución ("Processing") y valida la información y datos ingresados. La plataforma interpreta los parámetros del producto (tipo de síntesis, cantidad, escala, purificación, longitud y modificaciones 5' y 3') para realizar el cálculo automático de precios de acuerdo a la base de datos, o bien asigna una atención manual para productos especiales (como T4BRICK™ o T4GENE™ RNA).
</p>

**3. Análisis Bioinformático de Seguridad (Integración con BLAST)**
<p align="justify">
Como parte del control de calidad y sector salud, las secuencias ingresadas son analizadas de forma automática mediante la herramienta bioinformática BLAST (Basic Local Alignment Search Tool). El sistema compara la secuencia solicitada contra bases de datos biológicas registradas para evaluar el alineamiento, identidad y significancia estadística (como la detección de patógenos o secuencias del sector salud).
</p>

**4. Generación y Notificación Automática**
<p align="justify">
Una vez procesada la información, la plataforma gestiona el envío automático de notificaciones vía correo electrónico según el estado de la solicitud del usuario:
</p>
<p align="justify">
<ul style="text-align: justify;">
  <li><b>Envío de Ticket de Compra:</b> Genera de manera inmediata el desglose detallado de costos por producto (costo de secuencia, purificación, modificaciones y asignación de ID único de operación).</li>
  <li><b>Envío de Cotización Formal:</b> Adjunta el desglose económico en Excel, fechas sugeridas de pago y entrega, e instrucciones para la liquidación.</li>
  <li><b>Detección de secuencias, Notificación Blast (Sector Salud / BLAST):</b> En caso de detectar coincidencias de alta similitud en la base de datos biológica, el sistema redirige la solicitud al área de Síntesis para una revisión manual y evaluación de viabilidad previa al procesamiento.</li>
</ul>



### ¿Cómo lo hace?
<p align="justify">
   
   ---
   
### Tiempo de prueba
   <p align="justify">

Se realizaron dos revisiones de las cotizaciones en tiempos diferentes, la primera prueba fue de manera automática en la cual la plataforma de cotización recibía los formatos de llenado uno tras otro y se generaban los correos electrónicos con la respuesta de su cotización, esto para obtener una revisión previa de manera automatiada y rapida.
<p align="justify">
La segunda prueba se realizo de manera manual, esto para generar un registro mas especifico de los resultados, se hizo una prueba general con 411 formatos existentes de productos solicitados por usuarios, se cotizo en un periodo del 14 al 25 de septiembre, se hizo uso de la plataforma coT4 y el correo para la recepción de las cotizaciones, se cargo en la plataforma de uno por uno de los formatos y se realizo un registro en cuales se llevo a cabo la cotización de manera correcta y en cuales arrojo error, se reviso cada formato y verifico si fue por formato anterior o formato actualizado, también se registro los errores mas presentes por parte del usuario en el llenado del formato anterior y como se releja la solución en el nuevo formato cotizador.

---

**Resultados**

Las variaciones posibles:
<table>
  <tr>
    <th style="background-color: black; color: white;">Formato</th>
    <th style="background-color: black; color: white;">Cotización</th>
  </tr>
  <tr>
    <td style="background-color: #e99698;"><b>Anterior</b></td>
    <td style="background-color: #a9c5f0;"><b>Correcta</b></td>
  </tr>
  <tr>
    <td style="background-color: #efff80;"><b>Diferente</b></td>
    <td style="background-color: #efff80;"><b>Otro</b></td>
  </tr>
  <tr>
    <td style="background-color: #a9c5f0;"><b>Correcto</b></td>
    <td style="background-color: #e99698;"><b>Error</b></td>
  </tr>
</table>

* Formato Anterior: No cuenta con las listas desplegables

* Formato correcto: Cuenta los las listas desplegables y seguros para el correcto ingreso de información por el usuario


<img width="518" height="320" alt="Recuento de cotizaciones" src="https://github.com/user-attachments/assets/c8090ea2-aed7-4721-88f4-79d706ede965" />

<p align="justify">
De un total de 411 cotizaciones el 80.9% fueron correctas y cotizadas con éxito, las cuales corresponden a cotizaciones realizadas con el nuevo formato actualizado, el 19.1% restante fueron cotizaciones erróneas que fueron hechas con el formato antiguo.


<p align="justify">
   
También existen casos especiales en que la cotización no puede concluir de manera exitosa usando el formato anterior o actualizado
Ejemplos:
* Solicitud de productos no específicos del catálogo que requieren una cotización manual, ya sea que no se encuentren en la base de datos de cualquiera de los dos formatos.
* Modificaciones por el usuario del formato cotizador. Ej: Eliminar filas, agregar cuadros, etc.
* Valores o caracteres no válidos por el formato anterior

<img width="600" height="371" alt="Uso incorrecto del formato " src="https://github.com/user-attachments/assets/cde79fbb-21d1-4c77-8771-dcc0733c2bb1" />


El 8.5% del total de las cotizaciones presentan un error debido a alguna anomalía ajena al formato cotizador debido al uso incorrecto.

---

### Errores
<p align="justify">
El 19.1% de cotizaciones que no se pudieron concluir de manera exitosa y marcaron como error, presentan un patrón marcado en ser realizadas con el formato de llenado anterior, el cual no cuenta con las listas despegables y el usuario tenia mayor libertad para realizar el llenado de este que resulta de una manera incorrecta.

Del total de todas las cotizaciones erróneas solo se presento un caso en el cual el formato utilizado fue el actualizado y la cotización fue errónea, esto debido a una modificación en el formato en su estructura por parte del usuario

El resto de las cotizaciones erróneas corresponden al uso del formato anterior con modificaciones y llenado incorrecto con caracteres no validos.

Ejemplos de los errores mas rrecurrentes:

1. Solicitudes de productos que equieren de una cotización manual dado qe no se encuentran en la base de datos


<img width="1157" height="185" alt="image" src="https://github.com/user-attachments/assets/e5034764-359c-48ea-b249-c4db1d8ed0b6" />
<img width="1231" height="188" alt="image" src="https://github.com/user-attachments/assets/1ad9c543-5976-469a-b66c-b18b7d9c7148" />

2. Ingreso incompleto y caracteres no validos

<img width="915" height="336" alt="image" src="https://github.com/user-attachments/assets/ef60b13f-c9d5-40a7-983c-461d649b02d0" />

---

### Solución de problemas

<p align="justify">
Los errores mas frecuentes ya identificados por los cuales no es posible cerrar la cotización con éxito corresponden al formato cotizador anterior, las modificaciones realizadas en el formato actualizado  se diseñaron de manera que estos errores por parte del usuario ya no fueran posibles con la implementación de campos de llenado de caracter obligatorio, listas despegables y seguros.

<p align="center">
  <img width="1107" height="472" alt="image" src="https://github.com/user-attachments/assets/9f1200d8-7a70-4a5b-b367-47c504f2cc17" />
</p>


El nuevo formato al contar con las listas despegables no permitirá el ingreso de otra información que no se encuentre en la base de datos para la generación de la cotización, si el usuario desea un producto que no se encuentre en el catalogo de la lista posra conractar al equipo de ventas ya que requerira de una cotiación manual.

En el caso de ingreso de caracteres no validos también se ve restringido por el nuevo formato cotizador ya que contiene seguros y solo se podrá ingresar de manera correcta.

El uso exitoso del formato actualizado se puede reflejar en que el total de 411 cotizaciones el 80.9% fueron correctas y cotizadas con éxito, las cuales corresponden a cotizaciones realizadas con el nuevo formato actualizado y todas las cotizaciones realizadas con el nuevo formato actualizado fueron correctas a excepción de solo un formato el cual fue modificado en su estructura.  



