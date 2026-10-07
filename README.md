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
   
<p align="justify">
<li><b>Envío de Ticket de Compra:</b> Genera de manera inmediata el desglose detallado de costos por producto (costo de secuencia, purificación, modificaciones y asignación de ID único de operación).</li>
<li><b>Envío de Cotización Formal:</b> Adjunta el desglose económico en Excel, fechas sugeridas de pago y entrega, e instrucciones para la liquidación.</li>
<li><b>Detección de secuencias, Notificación Blast (Sector Salud / BLAST):</b> En caso de detectar coincidencias de alta similitud en la base de datos biológica, el sistema redirige la solicitud al área de Síntesis para una revisión manual y evaluación de viabilidad previa al procesamiento.</li>
</ul>



### ¿Cómo lo hace?
<p align="justify">
   
   ---
   
### Tiempo de prueba
   <p align="justify">

Se realizaron dos revisiones de las cotizaciones en tiempos diferentes, una de manera automatizada y otra de manera manual cada una con objetivos diferentes.

* ### Cotización automatizada

<p align="justify">
El objetivo de esta primera prueba fue para comprobar si la plataforma cumplía su función, verificar que los archivos pudieran ser procesados correctamente, que la información válida pudiera utilizarse para generar una cotización y detectar los principales errores que podían presentarse durante el proceso y como podía mejorarse, saber cuales son las métricas en tiempos de cotización y obtener un recuento de ls cotizaciones exitosas y erróneas.

   -- **Desarrollo de la prueba** --
   
<p align="justify">
La prueba se realizó mediante un flujo dividido en dos etapas principales:

**1.  Revisión de los formatos**

<p align="justify">
En esta etapa se procesaron los archivos de Excel del formato de llenado para comprobar que contaran con la información y estructura necesarias para que la plataforma pudiera continuar con la cotización.
   
<p align="justify">
Los archivos que cumplían con las condiciones requeridas continuaban al siguiente proceso, mientras que aquellos que presentaban alguna anomalía eran registrados como fallidos junto con la información disponible sobre el problema.

**2.  Generación de la cotización**

<p align="justify">
Los formatos que superaban la etapa de revisión pasaban al proceso de cálculo de la cotización. En esta etapa se procesaba la información del formato para generar el precio correspondiente.
   
<p align="justify">
Cada intento era registrado como completado o fallido. En los casos exitosos se registraba también el tiempo empleado para realizar el cálculo.


* ### Cotiación manual
  
<p align="justify">
Esta segunda prueba se realizo de manera manual con el objetivo de recaudar mayor información sobre el uso correcto e incorrecto del formato de llenado por parte del usuario y el uso del nuevo formato cotizador y su respuesta, esto para generar un registro mas especifico de los resultados.

-- **Desarrollo de la prueba** --

<p align="justify">
Se realizo una prueba general con un total de 411 formatos existentes de productos solicitados por usuarios, se cotizo en un periodo del 14 al 25 de septiembre, se hizo uso de la plataforma coT4 y el correo para la recepción de las cotizaciones 
   
<p align="justify">
Se cargo en la plataforma de uno por uno de los formatos y se realizo un registro en cuales se llevo a cabo la cotización de manera correcta y en cuales arrojo error segun los resultados obtenidos en por correo electronico, se reviso cada formato que sealo como cotizacion errones no concluida y se verifico si el formato cotizado correspondia al formato anterior o formato actualizado, también se registro los errores mas rrecurrentes por parte del usuario en el llenado del formato anterior.

---

### **Resultados**

* ### Cotización automatizada
  
De acuerdo con los registros de la prueba, se obtuvieron los siguientes resultados:


<img width="670" height="304" alt="image" src="https://github.com/user-attachments/assets/d3842552-8c7c-4822-9d44-0cb11607a273" />

Gráfico 1. Resultados de intentos registrados por etapa.

<p align="justify">
En la etapa de revisión se registraron 2,570 procesamientos completados correctamente y 90 con algún tipo de fallo. Posteriormente, durante la generación de cotizaciones, se registraron 1,385 procesos completados y 786 fallos.

* **Factores que impiden una cotización exitosa por la plataforma**

<p align="justify">
Durante la revisión de los formatos se identificaron 90 registros de fallo. Los problemas encontrados con mayor frecuencia fueron:

* Producto no localizado o nombre diferente al registrado en la base de datos: 37 casos.

* Información o estructura del archivo de Excel fuera de lo esperado: 32 casos.

* Campo o valor sin completar: 4 casos.

* Archivo que no correspondía a un formato de Excel: 4 casos.

* Formato incompleto: 1 caso.

* Problema interno al preparar una carpeta de trabajo: 12 casos.
  
<p align="justify">
Estos resultados permitieron identificar principalmente problemas relacionados con la información proporcionada en los formatos y con la estructura esperada por el sistema. También se identificaron algunos problemas internos del proceso que no necesariamente corresponden a errores del usuario.

**Tiempo de generación de las cotizaciones**

<p align="justify">
Para los 1,385 procesos de cotización que concluyeron correctamente, se registraron diferentes tiempos de ejecución:

* Mediana: 28 segundos.

* Promedio: 85.4 segundos.

* Tiempo mínimo: 3 segundos.

* Tiempo máximo: 14 horas, 29 minutos y 2 segundos.
  
<p align="justify">
La mediana de 28 segundos representa una referencia más cercana al tiempo de ejecución de un caso típico, mientras que el promedio se incrementó debido a algunos procesos que requirieron un tiempo considerablemente mayor. El caso de mayor duración se considera un comportamiento fuera de lo común ajeno al desempeño de la plataforma que podría requerir una revisión adicional.
   
<p align="justify">
Esta prueba automatizada permitió comprobar el funcionamiento del flujo de procesamiento de los formatos y de generación de cotizaciones, así como identificar los principales problemas que pueden impedir que una solicitud avance correctamente.
   
<p align="justify">
Los resultados muestran que la plataforma es capaz de procesar los formatos y generar cotizaciones en una parte importante de los casos evaluados. Asimismo, las pruebas permitieron detectar errores frecuentes relacionados principalmente con productos no identificados, información incompleta y formatos cuya estructura no corresponde con la esperada por el sistema.

* ### Cotización manual

De acuerdo con el registro que se realizo de manera manual, se obtuvieron los siguientes resultados:

Variaciones posibles:

<table>
  <tr>
    <th style="background-color: black; color: white;">Formato</th>
    <th style="background-color: black; color: white;">Cotización</th>
  </tr>
  <tr>
    <td style="background-color: #e99698;">Anterior</td>
    <td style="background-color: #a9c5f0;">Correcta</td>
  </tr>
  <tr>
    <td style="background-color: #efff80;">Diferente</td>
    <td style="background-color: #efff80;">Otro</td>
  </tr>
  <tr>
    <td style="background-color: #a9c5f0;">Correcto</td>
    <td style="background-color: #e99698;">Error</td>
  </tr>
</table>


* Formato Anterior: No cuenta con las listas desplegables

* Formato correcto: Cuenta los las listas desplegables y seguros para el correcto ingreso de información por el usuario


<img width="518" height="320" alt="Recuento de cotizaciones" src="https://github.com/user-attachments/assets/c8090ea2-aed7-4721-88f4-79d706ede965" />

Gráfico 2. Recuento de cotizaciones.


<p align="justify">
De un total de 411 cotizaciones el 80.9% fueron correctas y cotizadas con éxito, las cuales corresponden a cotizaciones realizadas con el nuevo formato actualizado, el 19.1% restante fueron cotizaciones erróneas que fueron hechas con el formato antiguo.


<p align="justify">
   
También existen casos especiales en que la cotización no puede concluir de manera exitosa usando el formato anterior o actualizado
Ejemplos:
* Solicitud de productos no específicos del catálogo que requieren una cotización manual, ya sea que no se encuentren en la base de datos de cualquiera de los dos formatos.
* Modificaciones por el usuario del formato cotizador. Ej: Eliminar filas, agregar cuadros, etc.
* Valores o caracteres no válidos por el formato anterior

<img width="600" height="371" alt="Uso incorrecto del formato " src="https://github.com/user-attachments/assets/cde79fbb-21d1-4c77-8771-dcc0733c2bb1" />

Gráfico 3. Uso incorrecto del formato.

El 8.5% del total de las cotizaciones presentan un error debido a alguna anomalía ajena al formato cotizador debido al uso incorrecto.

<p align="justify">
El 19.1% de cotizaciones que no se pudieron concluir de manera exitosa y marcaron como error en la plataforma, presentan un patrón marcado en ser realizadas con el formato de llenado anterior, el cual no cuenta con las listas despegables y el usuario tenia mayor libertad para realizar el llenado de este que resulta de una manera incorrecta.

Del total de todas las cotizaciones no concluidas solo se presento un caso en el cual el formato utilizado fue el actualizado y la cotización fue errónea, esto debido a una modificación en el formato en su estructura por parte del usuario

El resto de las cotizaciones erróneas o no concluidas corresponden al uso del formato anterior con modificaciones y llenado incorrecto con caracteres no validos.

* **Factores que impiden una cotización exitosa por la plataforma**

1. Solicitudes de productos que requieren de una cotización manual dado que no se encuentran en la base de datos de la plataforma

**Ejemplo:**

Figura 1.
<img width="1445" height="232" alt="imagen" src="https://github.com/user-attachments/assets/e552f215-04a0-42bf-bc4b-4d41cc92493d" />
Figura 2.
<img width="1535" height="230" alt="imagen" src="https://github.com/user-attachments/assets/85c83225-940e-4a28-8aea-0e8d42b28057" />

<p align="justify">
Este tipo de situaciones marcara como error por la plataforma y no precisamente porque sea  incorrecta la solicitud del uduario o sea imposible la cotización del producto solicitado, el problema persiste en que debido a que el cotizador funciona con productos previamente registrados en su base de datos, cuando el usuario solicita un producto que no se encuentra disponible en dicha base, el sistema no puede identificarlo y, por lo tanto, no puede generar automáticamente su cotización.

En estos casos, la solicitud debe ser atendida mediante una cotización manual, especialmente cuando se trata de productos especiales o que requieren una configuración que no se encuentra contemplada en el cotizador.

En el formato mostrado en la figura 1 y figura 2 se solicitaron los siguientes productos:
- GIGAscript™ RT
- NextPure ViroBac

Estos productos no se encuentran disponibles dentro de la base de datos utilizada por el cotizador, por lo que la plataforma no puede asociarlos con un producto registrado ni determinar automáticamente su precio.

2. Ingreso incorrecto y caracteres no validos

Figura 3.
<img width="1374" height="241" alt="imagen" src="https://github.com/user-attachments/assets/09bcd7a8-47c0-4c9e-8f83-7a18a86d0523" />

<p align="justify">
En este caso, la cotización no se realizó de manera exitosa debido a que el archivo de entrada no conservó la estructura y el formato establecido para el registro de modificaciones
Como se puede observar en la figura 3, en las columnas correspondientes a las modificaciones 5' y 3' fueron combinadas en una sola celda, eliminando la separación requerida entre ambos extremos de la secuencia. Esta estructura es necesaria para que la plataforma pueda interpretar de manera independiente la modificación correspondiente a cada extremo del oligo.


<img width="915" height="336" alt="image" src="https://github.com/user-attachments/assets/ef60b13f-c9d5-40a7-983c-461d649b02d0" />





---

### Solución de problemas

<p align="justify">
Los situaciones mas frecuentes ya identificados por los cuales no es posible cerrar la cotización con éxito corresponden al formato cotizador anterior, las modificaciones realizadas en el formato actualizado  se diseñaron de manera que estos errores por parte del usuario ya no fueran posibles con la implementación de campos de llenado de caracter obligatorio, listas despegables y seguros.
   
Figura 4. 
<p align="center">
  <img width="1107" height="472" alt="image" src="https://github.com/user-attachments/assets/9f1200d8-7a70-4a5b-b367-47c504f2cc17" />
</p>


El nuevo formato al contar con las listas despegables no permitirá el ingreso de otra información que no se encuentre en la base de datos para la generación de la cotización, si el usuario desea un producto que no se encuentre en el catalogo de la lista posra conractar al equipo de ventas ya que requerira de una cotiación manual.

En el caso de ingreso de caracteres no validos también se ve restringido por el nuevo formato cotizador ya que contiene seguros y solo se podrá ingresar de manera correcta.

El uso exitoso del formato actualizado se puede reflejar en que el total de 411 cotizaciones el 80.9% fueron correctas y cotizadas con éxito, las cuales corresponden a cotizaciones realizadas con el nuevo formato actualizado y todas las cotizaciones realizadas con el nuevo formato actualizado fueron correctas a excepción de solo un formato el cual fue modificado en su estructura.  



