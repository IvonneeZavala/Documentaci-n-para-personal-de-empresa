# Documentación para personal de la empresa
Una introducción a la plataforma coT4, qué es, su creación y funcionamiento.

### ¿Qué es la plataforma coT4? 

<p align="justify">
Cotizador en línea comercial diseñado para optimizar el proceso de venta y atención al cliente, una cotización inmediata que transforma rápidamente la solicitud del cliente en un ticket de compra a través de su correo electrónico.
</p>

Puede ingresar a la plataforma a través del siguiente link: https://docker.t4oligo.com/#:~:text=Acciones%20Principales%20Enviar%20Cotizaci%C3%B3n%20Limpiar%20Formulario

<p align="justify">
Para llevar a cabo su cotización, deberá ingresar y, como primer paso, se deberá descargar la plantilla del formato cotizador en el botón <strong>“Descargar plantilla”</strong> y se abrirá el Excel, el cual contiene diferentes apartados que se deben llenar de manera completa y correcta. Se observarán los apartados de <strong>“Datos de envío”</strong>, <strong>“Datos de facturación”</strong> y, seguido de estos, el apartado general para la solicitud del producto con sus especificaciones.
Para realizar un correcto llenado de este formato se recomienda leer previamente la <strong>"Guía de llenado del formato cotizador"</strong> que se le será disponible.
</p>
<p align="center">
  <img width="1364" height="655" alt="image" src="https://github.com/user-attachments/assets/3960cd46-1c4b-4145-9d6b-7355545f3fde" />
</p>

<p align="justify">
Al completar todas las casillas de su formato cotizador, deberá guardarse el Excel y cargarse a la página mediante el botón <strong>“Cargar desde Excel”</strong>, seguido del botón <strong>“Enviar cotización”</strong>.
</p>

Al oprimir el botón **“Enviar cotización”**, la interfaz deberá realizar las siguientes acciones:
1. Cambio en la velocidad de la animación de las letras **“A”**, **“T”**, **“C”** y **“G”**, aumentando su velocidad para indicar que el proceso se encuentra en ejecución.
2. Actualiación en el estado del proceso. La leyenda ubicada en la parte inferior, que inicialmente muestra **“READY”**, deberá cambiar a **“Processing”** mientras se procesa la solicitud.
<img width="1364" height="655" alt="image" src="https://github.com/user-attachments/assets/7e26eb9b-66d8-40dd-8a54-8a1299fb5639" />

3. Mostrar el resultado del proceso en la parte superior derecha de la interfaz

 * Si el archivo se carga correctamente, deberá aparecer un mensaje en la esquina superior derecha indicando: **“Archivo [Nombre del archivo] cargado correctamente”**.

<img width="1364" height="655" alt="image" src="https://github.com/user-attachments/assets/d076bcba-7455-4060-beea-a0cc64b589e5" />


 * Si ocurre un error durante la carga o el procesamiento, deberá mostrarse una pestaña en la parte superior derecha con una descripción del error y, cuando corresponda, el nombre del error.

Una vez finalizado el proceso, la interfaz deberá regresar a su estado inicial y la animación deberá volver a su velocidad lenta. 

Tras haber completado y enviado el formulario correctamente, el usuario recibirá una respuesta en su correo electrónico. Dependiendo del estado de su solicitud, puede recibir uno de los siguientes 3 tipos de notificación: 

1. Recepción de ticket de compra:
2. Recepción de la Cotización
3. Detección de secuencias, Notificación Blast (Sector Salud / BLAST)

---

<p align="justify">
Esta plataforma permite optimizar el flujo de información entre el cliente y las áreas involucradas en el proceso de cotización, reduciendo errores en la captura de datos, agilizando la revisión de las solicitudes y facilitando el seguimiento de cada requerimiento hasta la generación y envío de la cotización correspondiente.
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

---

### Versiones del formato cotizador: anterior y actualizado

<p align="justify">
Durante el uso de la plataforma coT4 se trabajó con dos versiones del formato cotizador: una versión anterior y una versión actualizada. Es importante distinguirlas ya que los resultados de las pruebas sobre la evaluación de la plataforma muestran diferencias entre los formatos utilizados y su relación con el éxito o los errores de las cotizaciones.
</p>

<p align="justify">
El formato anterior no contaba con listas desplegables ni con las mismas restricciones de entrada del formato actualizado. Por ello, el usuario tenía mayor libertad para escribir o modificar la información, lo que podía ocasionar registros con caracteres no válidos, datos ingresados de manera incorrecta o cambios en la estructura del archivo.
</p>

<p align="justify">
El formato actualizado incorporó listas desplegables, campos obligatorios y seguros para orientar y restringir el ingreso de información. Estos cambios se implementaron para reducir los errores de captura y facilitar que los datos mantuvieran la estructura esperada por la plataforma.
</p>

<p align="justify">
Esta diferencia debe tenerse en cuenta al interpretar los resultados que se presentan en el apartado de pruebas y resultados.
</p>

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
Al enviar el formulario, el sistema ajusta dinámicamente el estado del proceso a ejecución ("Processing") y valida la información y datos ingresados. La plataforma interpreta los parámetros del producto (tipo de síntesis, cantidad, escala, purificación, longitud y modificaciones 5' y 3') para realizar el cálculo automático de precios de acuerdo a la base de datos.
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
<li><b>Envío de Ticket de Compra:</b> Genera de manera inmediata el desglose detallado de costos por producto (costo de secuencia, purificación, modificaciones y asignación de ID único de operación).</li>
<li><b>Envío de Cotización Formal:</b> Adjunta el desglose económico en Excel, fechas sugeridas de pago y entrega, e instrucciones para la liquidación.</li>
<li><b>Detección de secuencias, Notificación Blast (Sector Salud / BLAST):</b> En caso de detectar coincidencias de alta similitud en la base de datos biológica, el sistema redirige la solicitud al área de Síntesis para una revisión manual y evaluación de viabilidad previa al procesamiento.</li>
</ul>

---

### ¿Cómo lo hace?

<p align="justify">
La plataforma COT4 procesa automáticamente el archivo de Excel proporcionado por el usuario para organizar, estandarizar y preparar la información de los productos solicitados para su cotización. Este proceso permite identificar los productos, unificar sus características y reconocer las modificaciones indicadas en cada registro.
</p>

El procesamiento se realiza mediante las siguientes etapas:

**1. Lectura del formato cotizador**

<p align="justify">
La plataforma abre el archivo de Excel y extrae las filas que contienen información de los productos solicitados. Identifica los campos correspondientes al tipo de producto, cantidad, nombre, secuencia, escala, purificación, número de bases y modificaciones en los extremos 5′ y 3′.
</p>
  
**2. Identificación del tipo de producto**

<p align="justify">
Con base en la información proporcionada, el sistema clasifica los registros en categorías como oligo estándar, oligo modificado o sonda. También reconoce determinadas categorías especiales, como RNA, T4BRICK™ y T4GENE™, así como algunos tipos de sondas con modificaciones específicas.
</p>

**3. Normalización de la información**

<p align="justify">
El sistema estandariza los datos para mantener un formato uniforme. Entre las acciones realizadas se encuentran:

- Convertir las secuencias a letras mayúsculas.
- Eliminar espacios innecesarios en los nombres y las secuencias.
- Sustituir los espacios de los nombres por guiones bajos.
- Unificar los nombres de los productos y las categorías correspondientes.
- Estandarizar la escritura de las escalas y los tipos de purificación.
</p>

**4. Asignación de valores predeterminados**

<p align="justify">
Cuando algunos campos de escala o purificación se encuentran vacíos, el sistema puede asignar valores predeterminados de acuerdo con la categoría del producto.
</p>

<p align="justify">
Por ejemplo, para los oligos estándar y modificados puede asignar una escala de 50 nmol y purificación por desalado. Para determinadas sondas puede establecer una escala de 200 nmol y purificación HPLC. En algunos productos especiales, los campos que no aplican se completan con el valor «No».
</p>

**5. Reconocimiento de modificaciones**

<p align="justify">
El sistema revisa las modificaciones indicadas en la secuencia y en sus extremos 5′ y 3′. Para ello, compara las etiquetas ingresadas con un catálogo de modificaciones previamente configurado.
</p>

<p align="justify">
Cuando identifica una modificación interna reconocida, puede registrarla en el campo correspondiente. Si no encuentra una coincidencia suficiente, el sistema puede marcarla como «No reconocido», lo que permite identificar información que requiere revisión.
</p>

**6. Preparación de la secuencia final**

<p align="justify">
Una vez procesados los datos, el sistema prepara la secuencia incorporando las modificaciones de los extremos 5′ y 3′ cuando corresponda. De esta manera, la información queda organizada para representar las características del producto solicitado.
</p>

**7. Organización y generación del resultado**

<p align="justify">
Finalmente, el sistema organiza los campos procesados y genera un archivo interno de los productos; este archivo almacena los resultados y los registra en la base de datos interna.
</p>

---

### Mejoras incorporadas en el formato cotizador actualizado

<p align="justify">
La actualización del formato cotizador se enfocó en prevenir errores frecuentes identificados durante el uso del formato anterior. Para ello, se incorporaron elementos que orientan al usuario al capturar la información y limitan ciertas entradas incorrectas antes de cargar el archivo en la plataforma.
</p>

**Cambios incorporados:**

<p align="justify">
  
- **Listas desplegables:** permiten seleccionar opciones disponibles en lugar de escribir libremente determinados datos, lo que ayuda a mantener la información alineada con las opciones configuradas para el cotizador.
- **Campos obligatorios:** ayudan a evitar que se envíe el formato con información requerida sin completar.
- **Seguros y restricciones de entrada:** limitan el ingreso de caracteres o valores no válidos en los campos configurados y reducen la posibilidad de capturar la información de manera incorrecta.
- **Conservación de la estructura del formato:** el uso de la plantilla actualizada busca que los datos permanezcan en las columnas y apartados esperados por la plataforma. Si el usuario elimina filas, agrega cuadros o cambia la estructura, aún pueden presentarse errores de procesamiento.
</p>

<p align="justify">
Estas mejoras reducen la libertad de modificar manualmente los campos que deben conservar un formato específico y ayudan a prevenir errores de captura. Sin embargo, no eliminan todos los casos que requieren revisión: los productos especiales o aquellos que no se encuentran en la base de datos pueden necesitar una cotización manual por parte del equipo de ventas.
</p>

---

### Pruebas y evaluación del formato cotizador

<p align="justify">
Se realizaron dos revisiones de las cotizaciones en tiempos diferentes, una de manera automatizada y otra de manera manual cada una con objetivos diferentes.
</p>

* ### Cotización automatizada
  
<p align="justify">
La prueba se ejecutó de manera automatizada mediante la computadora, utilizando un procedimiento programado para evaluar el funcionamiento de la plataforma y el procesamiento de los formatos de cotización. A diferencia de una prueba manual, en la que cada formato se carga y verifica individualmente por una persona, la prueba automatizada permite ejecutar múltiples casos de prueba de forma sistemática y registrar los resultados obtenidos.
</p>

<p align="justify">
El objetivo de esta primera prueba fue para comprobar si la plataforma cumplía su función, verificar que los archivos pudieran ser procesados correctamente, que la información válida pudiera utilizarse para generar una cotización y detectar los principales errores que podían presentarse durante el proceso y como podía mejorarse, saber cuales son las métricas en tiempos de cotización y obtener un recuento de las cotizaciones exitosas y erróneas.
</p>

-- **Desarrollo de la prueba** --

<p align="justify">
La prueba se realizó mediante un flujo dividido en dos etapas principales con un total de 4,831 intentos en total:
</p>

**1. Revisión de los formatos**

<p align="justify">
En esta etapa se procesaron los archivos de Excel del formato de llenado para comprobar que contaran con la información y estructura necesarias para que la plataforma pudiera continuar con la cotización.
</p>

<p align="justify">
Los archivos que cumplían con las condiciones requeridas continuaban al siguiente proceso, mientras que aquellos que presentaban alguna anomalía eran registrados como fallidos junto con la información disponible sobre el problema.
</p>

**2. Generación de la cotización**

<p align="justify">
Los formatos que superaban la etapa de revisión pasaban al proceso de cálculo de la cotización. En esta etapa se procesaba la información del formato para generar el precio correspondiente.
</p>

<p align="justify">
Cada intento era registrado como completado o fallido. En los casos exitosos se registraba también el tiempo empleado para realizar el cálculo.
</p>

* ### Cotización manual

<p align="justify">
Esta segunda prueba se realizo de manera manual con el objetivo de recaudar mayor información sobre el uso correcto e incorrecto del formato de llenado por parte del usuario y el uso del nuevo formato cotizador y su respuesta, esto para generar un registro mas especifico y hacer una revisión puntualmente de casos en los que se presento error e identificar el formato utilizado en dichas cotizaciones.
</p>

-- **Desarrollo de la prueba** --

<p align="justify">
Se realizo una prueba general con un total de 411 formatos existentes de productos solicitados por usuarios, se cotizo en un periodo del 14 al 25 de septiembre de 2026, se hizo uso de la plataforma coT4 y el correo para la recepción de las cotizaciones.
</p>


<p align="justify">
Se cargaron los formatos en la plataforma uno por uno y se llevó a cabo un registro de aquellos en los que la cotización se realizó correctamente y de aquellos en los que se presentó un error, de acuerdo con los resultados recibidos por correo electrónico. Se revisó cada formato señalado como una cotización errónea o no concluida, y se verificó si correspondía al formato anterior o al formato actualizado. Asimismo, se registraron los errores más recurrentes cometidos por los usuarios al llenar el formato anterior.
</p>

---

### **Resultados**

* ### Cotización automatizada

De acuerdo con los registros de la prueba, se obtuvieron los siguientes resultados:

<img width="670" height="304" alt="image" src="https://github.com/user-attachments/assets/277d0439-b046-4da8-9a96-9a2e2cbc97ab" />

**Gráfico 1. Resultados de intentos registrados por etapa.**

<p align="justify">
En la etapa de revisión se registraron 2,570 procesamientos completados correctamente y 90 con algún tipo de fallo. Posteriormente, durante la generación de cotizaciones, se registraron 1,385 procesos completados y 786 fallos.
</p>

* **Factores que impiden una cotización exitosa por la plataforma**

<p align="justify">
Durante la revisión de los formatos se identificaron 90 registros de fallo. Los problemas encontrados con mayor frecuencia fueron:
</p>

- Producto no localizado o nombre diferente al registrado en la base de datos: 37 casos.
- Información o estructura del archivo de Excel fuera de lo esperado: 32 casos.
- Campo o valor sin completar: 4 casos.
- Archivo que no correspondía a un formato de Excel: 4 casos.
- Formato incompleto: 1 caso.
- Problema interno al preparar una carpeta de trabajo: 12 casos.

<p align="justify">
Estos resultados permitieron identificar principalmente problemas relacionados con la información proporcionada en los formatos y con la estructura esperada por el sistema. También se identificaron algunos problemas internos del proceso que no necesariamente corresponden a errores del usuario.
</p>

**Tiempo de generación de las cotizaciones**

<p align="justify">
Para los 1,385 procesos de cotización que concluyeron correctamente, se registraron diferentes tiempos de ejecución:
</p>

- Mediana: 28 segundos.
- Promedio: 85.4 segundos.
- Tiempo mínimo: 3 segundos.
- Tiempo máximo: 14 horas, 29 minutos y 2 segundos.

<p align="justify">
La mediana de 28 segundos representa una referencia más cercana al tiempo de ejecución de un caso típico, mientras que el promedio se incrementó debido a algunos procesos que requirieron un tiempo considerablemente mayor. El caso de mayor duración se considera un comportamiento fuera de lo común ajeno al desempeño de la plataforma que podría requerir una revisión adicional.
</p>

<p align="justify">
Esta prueba automatizada permitió comprobar el funcionamiento del flujo de procesamiento de los formatos y de generación de cotizaciones, así como identificar los principales problemas que pueden impedir que una solicitud avance correctamente.
</p>

<p align="justify">
Los resultados muestran que la plataforma es capaz de procesar los formatos y generar cotizaciones en una parte importante de los casos evaluados. Asimismo, las pruebas permitieron detectar errores frecuentes relacionados principalmente con productos no identificados, información incompleta y formatos cuya estructura no corresponde con la esperada por el sistema.
</p>

* ### Cotización manual

De acuerdo con el registro que se realizó de manera manual, se obtuvieron los siguientes resultados:

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

- Formato Anterior: No cuenta con las listas desplegables.
- Formato correcto: Cuenta los las listas desplegables y seguros para el correcto ingreso de información por el usuario.

<img width="518" height="320" alt="Recuento de cotizaciones" src="https://github.com/user-attachments/assets/c8090ea2-aed7-4721-88f4-79d706ede965" />


**Gráfico 2. Recuento de cotizaciones.**

<p align="justify">
De un total de 411 cotizaciones el 80.9% fueron correctas y cotizadas con éxito, las cuales corresponden a cotizaciones realizadas con el nuevo formato actualizado, el 19.1% restante fueron cotizaciones erróneas que fueron hechas con el formato anterior.
</p>

<p align="justify">
También existen casos especiales en que la cotización no puede concluir de manera exitosa usando el formato anterior o actualizado.
</p>

Ejemplos:
- Solicitud de productos no específicos del catálogo que requieren una cotización manual, ya sea que no se encuentren en la base de datos de cualquiera de los dos formatos.
- Modificaciones por el usuario del formato cotizador. Ej: Eliminar filas, agregar cuadros, etc.
- Valores o caracteres no válidos por el formato anterior.

<img width="600" height="371" alt="Uso incorrecto del formato " src="https://github.com/user-attachments/assets/cde79fbb-21d1-4c77-8771-dcc0733c2bb1" />

**Gráfico 3. Uso incorrecto del formato.**

El 8.5% del total de las cotizaciones presentan un error debido a alguna anomalía ajena al formato cotizador debido al uso incorrecto.

<p align="justify">
El 19.1% de cotizaciones que no se pudieron concluir de manera exitosa y marcaron como error en la plataforma, presentan un patrón marcado en ser realizadas con el formato de llenado anterior, el cual no cuenta con las listas despegables y el usuario tenia mayor libertad para realizar el llenado de este que resulta de una manera incorrecta.
</p>

<p align="justify">
Del total de todas las cotizaciones no concluidas solo se presento un caso en el cual el formato utilizado fue el actualizado y la cotización fue errónea, esto debido a una modificación en el formato en su estructura por parte del usuario, específicamente una combinación de celdas lo cual hizo que la base de datos no pudiera reconocer los datos ingresados, sin embargo fue el único caso de error de cotización con el uso del formato nuevo actualiado.
</p>

<p align="justify">
El resto de las cotizaciones erróneas o no concluidas corresponden al uso del formato anterior con modificaciones y llenado incorrecto con caracteres no validos.
</p>

* **Factores que impiden una cotización exitosa por la plataforma**


**1. Solicitudes de productos que requieren de una cotización manual dado que no se encuentran en la base de datos de la plataforma.**

**Ejemplo:**

**Figura 1.**
<img width="1445" height="232" alt="imagen" src="https://github.com/user-attachments/assets/e552f215-04a0-42bf-bc4b-4d41cc92493d" />

**Figura 2.**
<img width="1535" height="230" alt="imagen" src="https://github.com/user-attachments/assets/85c83225-940e-4a28-8aea-0e8d42b28057" />

<p align="justify">
Este tipo de situaciones marcara como error por la plataforma y no precisamente porque sea incorrecta la solicitud del usuario o sea imposible la cotización del producto solicitado, el problema persiste en que debido a que el cotizador funciona con productos previamente registrados en su base de datos, cuando el usuario solicita un producto que no se encuentra disponible en dicha base, el sistema no puede identificarlo y, por lo tanto, no puede generar automáticamente su cotización.
</p>

<p align="justify">
En estos casos, la solicitud debe ser atendida mediante una cotización manual, especialmente cuando se trata de productos especiales o que requieren una configuración que no se encuentra contemplada en el cotizador.
</p>

<p align="justify">
En el formato mostrado en la figura 1 y figura 2 se solicitaron los siguientes productos:
</p>

- GIGAscript™ RT
- NextPure ViroBac

<p align="justify">
Estos productos no se encuentran disponibles dentro de la base de datos utilizada por el cotizador, por lo que la plataforma no puede asociarlos con un producto registrado ni determinar automáticamente su precio.
</p>

**2. Ingreso incorrecto y caracteres no validos**

**Figura 3.**
<img width="1374" height="241" alt="imagen" src="https://github.com/user-attachments/assets/09bcd7a8-47c0-4c9e-8f83-7a18a86d0523" />


<p align="justify">
En este caso, la cotización no se realizó de manera exitosa debido a que el archivo de entrada no conservó la estructura y el formato establecido para el registro de modificaciones. Como se puede observar en la figura 3, en las columnas correspondientes a las modificaciones 5' y 3' fueron combinadas en una sola celda, eliminando la separación requerida entre ambos extremos de la secuencia. Esta estructura es necesaria para que la plataforma pueda interpretar de manera independiente la modificación correspondiente a cada extremo del oligo.
</p>

---

### Solución de problemas, mejoras implementadas en el nuevo formato cotizador

<p align="justify">
Los situaciones mas frecuentes ya identificados por los cuales no es posible cerrar la cotización con éxito corresponden al formato cotizador anterior, las modificaciones realizadas en el formato actualizado se diseñaron de manera que estos errores por parte del usuario ya no fueran posibles con la implementación de campos de llenado de caracter obligatorio, listas despegables y seguros.
</p>

**Figura 4. Formato cotizador actualizado.**

<p align="center">
  <img width="1107" height="472" alt="image" src="https://github.com/user-attachments/assets/9f1200d8-7a70-4a5b-b367-47c504f2cc17" />
</p>

<p align="justify">
El nuevo formato al contar con las listas despegables no permitirá el ingreso de otra información que no se encuentre en el catálogo de la lista. Si el usuario desea un producto que no se encuentre en el catálogo, podrá contactar al equipo de ventas, ya que requerirá de una cotización manual.
</p>

<p align="justify">
El uso exitoso del formato actualizado se puede reflejar en que del total de 411 cotizaciones, el 80.9% fueron correctas y cotizadas con éxito, las cuales corresponden a cotizaciones realizadas con el nuevo formato actualizado.
</p>

### Conclusiones y beneficios de las mejoras implementadas
<p align="justify">
A partir de las pruebas automatizadas, las pruebas manuales y el análisis de los errores identificados durante el uso de la plataforma coT4, se determinó que el formato cotizador actualizado es un elemento fundamental para el correcto procesamiento de las solicitudes y la generación de cotizaciones.
</p>
  
<p align="justify">
La comparación entre la versión anterior y la versión actualizada del formato permitió identificar áreas de oportunidad relacionadas con la captura de información, la selección de productos y el cumplimiento de la estructura requerida por la plataforma.
</p>

<p align="justify">
Como respuesta a estas áreas de oportunidad, se incorporaron listas desplegables, campos obligatorios y validaciones que orientan al usuario durante el llenado del formato y ayudan a prevenir errores de captura, modificaciones no permitidas y solicitudes con información incompleta. Estas mejoras buscan estandarizar la información recibida y facilitar su procesamiento automático.
</p>

<p align="justify">
Asimismo, las pruebas realizadas permitieron identificar situaciones que requieren atención adicional, como las solicitudes de productos que no se encuentran registrados en la base de datos y los formatos cuya estructura ha sido modificada. En estos casos, es necesario revisar la información y, cuando corresponda, gestionar una cotización manual o solicitar al usuario que corrija el formato conforme a la guía establecida.
</p>

<p align="justify">
Finalmente, se comprobó que la actualización del formato cotizador representa una mejora en el control y la estandarización de los datos de entrada, contribuyendo a reducir errores atribuibles al llenado incorrecto y a facilitar el proceso de generación de cotizaciones. 
</p>
