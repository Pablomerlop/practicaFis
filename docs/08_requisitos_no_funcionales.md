# 8. Requisitos No Funcionales 

A continuación se detallan 10 requisitos que definen las restricciones y atributos de calidad del sistema, organizados según el modelo FURPS+ y la clasificación de Sommerville, y redactados mediante métricas verificables objetivamente.

### Usabilidad (Usability)
* **RNF-01 (Tiempo de entrenamiento):** El tiempo máximo de formación necesario para que un vigilante opere la aplicación móvil de forma autónoma debe ser inferior a 1 hora.
* **RNF-02 (Facilidad de uso):** La interfaz móvil debe estar diseñada de manera que la tasa de errores operativos cometidos por un usuario sea inferior a 2 errores por cada 100 interacciones.
* **RNF-03 (Eficiencia en el cambio de estado):** La interfaz web debe permitir al Responsable de RRHH completar el proceso de cambio de estado a "Activo" en un máximo de 3 clics desde la ficha principal del empleado.

### Rendimiento (Performance)
* **RNF-04 (Tiempo de respuesta):** El tiempo de respuesta máximo del sistema central ante una consulta de un operador (ej. buscar a un residente en el padrón) no debe superar los 2 segundos.
* **RNF-05 (Velocidad de procesamiento):** El servidor deberá ser capaz de procesar un mínimo de 50 transacciones por segundo en carga pico sin que el rendimiento se degrade.
### Fiabilidad (Reliability)
* **RNF-06 (Disponibilidad):** La probabilidad de que el sistema central no esté disponible para atender incidencias debe ser inferior al 0,1% mensual (Disponibilidad del 99,9%).
* **RNF-07 (Tiempo medio entre fallos - MTBF):** El sistema debe garantizar un tiempo medio de operación ininterrumpida sin fallos críticos superior a 720 horas.
* **RNF-08 (Tiempo de procesamiento de estado):** El sistema central debe procesar el cambio de estado y actualizar la disponibilidad del empleado en la base de datos en un tiempo máximo de 2 segundos.

### Robustez y Mantenibilidad (Supportability / Robustness)
* **RNF-09 (Tiempo de recuperación):** En caso de producirse un fallo grave o caída del servidor, el tiempo de arranque y restauración total del sistema no debe superar los 15 minutos.

### Requisitos "+" y Externos (Seguridad, Interoperabilidad y Legislativos)
* **RNF-10 (Seguridad / Protección - Sommerville):** Todas las comunicaciones y transmisiones de datos entre las aplicaciones cliente (web y móvil) y el servidor deberán estar cifradas utilizando el estándar AES-256.
* **RNF-11 (Requisito de Interfaz / Interoperabilidad):** La aplicación móvil enviará las coordenadas del incidente a la app de navegación GPS predeterminada del dispositivo en menos de 1 segundo utilizando los comandos (URI schemes) nativos del sistema operativo.
* **RNF-12 (Legislativo - Sommerville):** El sistema deberá almacenar y proteger los datos de carácter personal de los residentes y empleados cumpliendo estrictamente con el Reglamento General de Protección de Datos (RGPD) 2016/679 de la UE, impidiendo el acceso a los registros médicos y personales a perfiles no autorizados.
* **RNF-13 (Privacidad del justificante médico):** El archivo adjunto que contiene el parte de alta médica debe almacenarse cifrado mediante el estándar AES-256, garantizando el cumplimiento del RGPD al tratarse de información de salud confidencial.
