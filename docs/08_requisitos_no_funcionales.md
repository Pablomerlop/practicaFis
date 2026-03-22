# 8. Requisitos No Funcionales (Métricas Verificables)

#### RNF-01: Facilidad de uso (Usabilidad)
* **Tiempo de entrenamiento:** El tiempo máximo de formación necesario para que un vigilante opere la aplicación móvil de forma autónoma debe ser inferior a 1 hora.
* **Tasa de errores:** La interfaz debe estar diseñada de manera que el número máximo de errores operativos cometidos por un usuario sea inferior a 2 errores por cada 100 interacciones.

#### RNF-02: Velocidad y Rendimiento (Performance)
* **Tiempo de respuesta:** El tiempo de respuesta máximo del sistema central ante una consulta de un operador (ej. buscar a un residente) debe ser de 2 segundos.
* **Procesamiento de transacciones:** El servidor debe ser capaz de procesar un mínimo de 50 transacciones por segundo sin que el rendimiento se degrade.

#### RNF-03: Fiabilidad (Reliability)
* **Disponibilidad:** La probabilidad de que el sistema central no esté disponible debe ser inferior al 0,1% mensual.
* **Tiempo medio entre fallos (MTBF):** El sistema debe garantizar un tiempo medio de operación ininterrumpida sin fallos críticos superior a 720 horas.

#### RNF-04: Robustez (Robustness)
* **Tiempo de recuperación:** En caso de producirse un fallo grave o caída del servidor, el tiempo de arranque y restauración total del sistema no debe superar los 15 minutos.
* **Integridad de los datos:** La probabilidad de corrupción o pérdida de datos tras un fallo del sistema debe ser inferior al 0,01%.

#### RNF-05: Requisitos "+" (Seguridad, Interoperabilidad y Legales - Sommerville)
* **Seguridad y Privacidad (Control de acceso):** El sistema debe garantizar que cada empleado vea solo lo necesario para su trabajo. Se deben crear roles estrictos (Dirección, Jefe de Seguridad, Operador, Vigilante y RRHH) para proteger la información.
* **Interoperabilidad (Integración con mapas):** La aplicación móvil debe poder conectarse de forma fluida con el navegador GPS del propio teléfono para guiar rápidamente al vigilante hasta el lugar de la incidencia.
* **Requisitos Legales / Normativos:** El sistema debe tener en cuenta las leyes de seguridad privada, incluyendo una función obligatoria que controle la vigencia de las habilitaciones profesionales de los vigilantes.