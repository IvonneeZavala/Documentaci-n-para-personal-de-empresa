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


### ¿Cómo funciona la plataforma?

<p align="justify">
La plataforma opera como un flujo de trabajo digital automatizado que procesa solicitudes de cotización desde la captura inicial de datos por parte del cliente hasta el procesamiento completo.
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

<ul style="text-align: justify;">
  <li><b>Emisión de Ticket de Compra:</b> Genera de manera inmediata el desglose detallado de costos por producto (costo de secuencia, purificación, modificaciones y asignación de ID único de operación).</li>
  <li><b>Envío de Cotización Formal:</b> Adjunta el desglose económico en Excel, fechas sugeridas de pago y entrega, e instrucciones para la liquidación.</li>
  <li><b>Alerta de Revisión Técnica (Sector Salud / BLAST):</b> En caso de detectar coincidencias de alta similitud en la base de datos biológica, el sistema redirige la solicitud al área de Síntesis para una revisión manual y evaluación de viabilidad previa al procesamiento.</li>
</ul>

### ¿Cómo lo hace?
