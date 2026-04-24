# 6. Requisitos de información

## RI - 01: Empleados

El sistema debe almacenar la información de todos los empleados (vigilantes y personal de central), incluyendo:

1. **Datos personales**: nombre completo, fecha de nacimiento, DNI, domicilio y teléfonos de contacto.

2. **Datos laborales:** fecha de alta en la empresa, categoría profesional, el turno de preferencia para ser asignado y estado de la habilitación profesional (fecha de caducidad). 

3. **Situación actual:** activo, de baja (médica o de cualquier otro tipo), vacaciones o excedencia.

## RI - 02: Vehículos

El sistema debe almacenar la siguiente información de cada vehículo:

1. **Identificación**: matrícula, marca, modelo y año de compra.

2. **Uso y kilometraje**: kilómetros totales recorridos.

3. **Disponibilidad**: estado actual del vehículo (operativo, averiado o en taller) para evitar conflictos en la asignación de patrullas.

## RI - 03: Residentes

El sistema debe almacenar la siguiente información de cada residente:

1. **Identificación**: nombre completo y DNI o NIE.

2. **Ubicación**: Urbanización a la que pertenece y dirección completa de la vivienda.

3. **Contacto**: Lista de números asociados a la vivienda (fijos y móviles).

## RI - 04: Incidencias

El sistema debe almacenar la siguiente información de cada incidencia:

1. **Datos de apertura**: identificación del informante (residente identificado o datos de quien llama si es externo), urbanización y dirección donde ocurre el incidente, tipo de incidencia (alarma de intrusión activada, alarma de humo, accidente, problema de causa natural, solicitud de asistencia general u otro), descripción libre del problema contado por el residente, la fecha y hora y el estado de la incidencia (abierta, asignada o resuelta).

2. **Gestión y respuesta**: vigilante asignado (su identificación), registro de la confirmación de recepción y horas de salida y llegada al lugar.

3. **Resolución y cierre**: tipo definitivo del incidente, descripción de lo que encontró, solución adoptada, indicación de si requiere seguimiento posterior y hora de resolución.

## RI - 05: Urbanizaciones

El sistema debe almacenar la siguiente información de las comunidades de propietarios gestionadas:

1. **Identificación y características:** nombre de la urbanizacion, dimensiones y características particulares (si es tranquila, si tiene mucho movimiento, si es muy cerrada...)

2. **Datos del contrato**: número de patrullas semanales y tiempos de respuesta comprometidos ante incidencias.

3. **Alarmas de zonas comunes**: listado de las alarmas instaladas en el perímetro o zonas compartidas (vallas, club social, entrada), incluyendo su identificador y sus coordenadas GPS exactas.

## RI - 06: Datos de Alta Médica

El sistema deberá almacenar la información vinculada al Alta Médica, incluyendo:

1. **Fecha** efectiva de reincorporación al puesto.

2. **Identificador** del usuario de RRHH que registra el alta.

3. El **archivo** digital del justificante médico.

## RI - 07: Historial de Estados del Empleado

El sistema deberá mantener un Historial de Estados, almacenando para cada cambio:

1. El **estado anterior** (Ej. De baja).

2. El **nuevo estado** (Ej. Activo).

3. La **fecha y la hora** exacta en la que se produjo la modificación.

## RI - 08: Planificación de Turnos y Patrullas

El sistema debe almacenar la organización semanal del servicio operativo, incluyendo:

1. **Turnos**: registro de las cuatro franjas horarias fijas (0:00-6:00, 6:00-12:00, 12:00-18:00, 18:00-0:00) para cada uno de los 365 días del año.

2. **Patrullas**: asignación concreta de una patrulla a un turno y a una urbanización, la cual estará compuesta obligatoriamente por un vigilante responsable y un vehículo específico.

3. **Kilometraje**: el registro de kilómetros al inicio y al finalizar cada turno (apuntados por el vigilante).

## RI - 09: Alarmas de Viviendas

El sistema debe registrar de forma independiente las alarmas instaladas en domicilios privados, almacenando:

1. **Identificador**: código único de la alarma.

2. **Ubicación**: vivienda a la que está asociada.

3. **Tipo de alarma:** intrusión, humo o botón de pánico.

## RI - 10: Informantes Externos

Para gestionar los avisos dados por personas que no residen en las urbanizaciones (visitas, repartidores, etc.) que no figuran en la base de datos de clientes, el sistema debe registrar temporalmente:

1. **Datos de contacto manual**: nombre aportado y número de teléfono desde el que se realiza la llamada.

## RI - 11: Periodos de Ausencias y Vacaciones

Para evitar conflictos en la asignación de patrullas, el sistema debe registrar los periodos de inactividad de los empleados, incluyendo:

1. **Datos del periodo**: fecha de inicio y fecha de fin prevista.

2. **Tipo de ausencia**: vacaciones, baja médica, baja de otro tipo, o excedencia.

## RI - 12: Usuarios del Sistema y Roles

Para garantizar la seguridad y el control de acceso, el sistema debe almacenar las credenciales de los usuarios, incluyendo:

1. **Identificación de acceso**: usuario y contraseña.

2. **Rol/Perfil**: Director General, Jefe de Seguridad, Operador, Vigilante o RRHH, que determina los permisos de acceso a la información.
