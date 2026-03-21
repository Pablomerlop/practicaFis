# 11. Descripción textual de los casos de uso

A continuación, se detallan las especificaciones textuales de los procesos elementales de negocio necesarios para el registro y apertura de nuevas incidencias en el sistema.

---

### CU-01: Identificar residente (o informante)

**Descripción y disparador:** El sistema debe comportarse tal como se describe en este caso de uso cuando el Operador de Central recibe una llamada telefónica para dar un aviso y necesita saber quién está llamando y desde dónde, paso previo a la apertura de una incidencia.
**Precondición:** El actor Operador de Central está autenticado en el sistema.

**Secuencia normal:**
1. El Operador de Central descuelga la llamada e inicia el proceso de identificación.
2. El sistema captura automáticamente el número de teléfono entrante.
3. El sistema busca dicho número de teléfono en el padrón de residentes registrados.
4. El sistema encuentra una coincidencia y muestra en pantalla los datos asociados: nombre del residente, dirección completa de la vivienda y urbanización a la que pertenece.
5. El Operador de Central confirma verbalmente con la persona que llama que los datos mostrados son correctos.
6. El caso de uso finaliza con éxito.

**Poscondición escenarios éxito:**
El informante ha sido identificado inequívocamente en el sistema y sus datos están disponibles para ser utilizados en la gestión de alertas.

**Alternativas y excepciones:**
* **1a, 5a-** Si el Operador cancela el proceso o se corta la llamada, el caso de uso finaliza (quedando sin efecto).
* **4a-** Si el sistema no encuentra el número de teléfono, el Operador busca manualmente en el sistema por nombre o dirección. Si lo encuentra y el número es nuevo, se realiza el caso de uso "Registrar nuevo teléfono", y a continuación el caso de uso continúa por el paso 5.
* **4b-** Si el Operador tampoco encuentra a la persona mediante la búsqueda manual (es un informante externo, visita, etc.), el Operador introduce manualmente los datos básicos aportados (nombre y teléfono) y el caso de uso continúa por el paso 6.

---

### CU-02: Crear incidencia

**Descripción y disparador:** El sistema deberá comportarse tal como se describe en este caso de uso cuando se necesite registrar oficialmente una anomalía o emergencia, ya sea disparada por un actor humano (Operador o Vigilante) o por el Sistema de Alarmas.
**Precondición:** Si el disparador es un actor humano, este debe estar previamente autenticado en el sistema.

**Secuencia normal:**
1. El actor inicia el proceso de registro de una nueva incidencia.
2. Se realiza el caso de uso "Identificar residente".
3. El actor introduce los datos reportados: tipo de incidencia (alarma de intrusión, humo, accidente, causa natural, asistencia u otro), urbanización y dirección exacta donde ocurre el incidente, descripción libre del problema y la fecha/hora.
4. El sistema valida que los datos introducidos son correctos, genera un identificador único y registra la incidencia en estado "Abierta".
5. Se realiza el caso de uso "Asignar vigilante de patrulla".
6. El caso de uso finaliza.

**Poscondición escenarios éxito:**
El sistema ha creado un nuevo registro de incidencia con todos sus datos detallados (incluyendo la ubicación exacta) y ha derivado el problema a un vigilante.

**Alternativas y excepciones:**
* **1a, 3a-** Si el actor cancela el registro manual, el caso de uso finaliza (quedando sin efecto).
* **1b- (Disparador por Sistema de Alarmas):** Si el inicio del caso de uso es disparado automáticamente por el Sistema de Alarmas, el sistema extrae automáticamente el identificador, el tipo y la ubicación sin necesidad de realizar el paso 2 ni el paso 3, registra directamente la incidencia (paso 4) y el caso de uso continúa por el paso 5.
* **4a-** Si el sistema detecta que faltan campos obligatorios por rellenar, emite un mensaje informativo de error en pantalla solicitando los datos y el caso de uso continúa por el paso 3.