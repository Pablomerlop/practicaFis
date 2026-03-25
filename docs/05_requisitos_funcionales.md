# 5. Requisitos funcionales

## RF - 01: Planificación de turnos y patrullas

El sistema debe permitir al Jefe de Seguridad organizar semanalmente las patrullas, asignando vigilantes y vehículos específicos a cada turno y urbanización.


## RF - 02: Visualización de recursos en tiempo real

El sistema debe mostrar en un panel la ubicación geográfica actualizada de todos los vigilantes y vehículos que se encuentren de servicio, permitiendo identificar visualmente su estado de disponibilidad (disponible, asignado a incidencia o fuera de servicio).

## RF - 03: Identificación automática de residentes

Al recibir una llamada, el sistema debe permitir identificar al residente (nombre, dirección y urbanización) a través de su número de teléfono, incluso si hay varios números asociados a una misma vivienda.

## RF - 04: Gestión y apertura de incidencias

El sistema debe permitir a los operadores crear incidencias registrando el informante, la ubicación, el tipo de incidente (intrusión, humo, accidente, etc.), una descripción libre y la fecha y hora.

## RF - 05: Registro automático de alarmas

El sistema debe registrar automáticamente como incidencias los disparos de alarmas de intrusión o humo conectadas a la central, identificando la vivienda o las coordenadas GPS en caso de alarmas perimetrales.

## RF - 06: Generación de informes de rendimiento y actividad

El sistema debe generar reportes mensuales y estadísticas que incluyan el número de incidencias, tiempos de respuesta y alarmas disparadas.

## RF - 07: Gestión de base de datos de residentes

El sistema debe permitir a los operadores de la central realizar el alta, baja y modificación de los datos de los residentes , asociando a cada vivienda el nombre del titular, su DNI/NIE y la lista completa de teléfonos de contacto autorizados.

## RF - 08: Alerta por falta de respuesta del vigilante

El sistema debe monitorizar el tiempo de respuesta tras la asignación de una incidencia y emitir una alerta automática a la central si el vigilante no confirma la recepción del aviso en un plazo superior a dos minutos.

## RF - 09: Control de vigencia de habilitaciones profesionales

El sistema debe monitorizar las fechas de validez de la habilitación profesional de cada vigilante y generar avisos automáticos al departamento de RRHH con antelación a su caducidad para evitar problemas legales en la asignación de turnos.

## RF - 10: Informe de resolución de una incidencia

El sistema debe permitir al vigilante asignado registrar el informe de resolución de una incidencia, incluyendo el tipo definitivo del incidente, descripción de lo que encontró, solucion adoptada y hora de resolución.

## RF - 11: Validación de estado previo del empleado

El sistema debe validar que el estado actual del empleado seleccionado sea "De baja" antes de permitir al usuario iniciar el proceso de registro de alta médica.

## RF - 12: Notficación automática de reincorporación

El sistema debe enviar una notificación automática al Jefe de Seguridad en el mismo momento en que el empleado pasa a estar "Activo", para que pueda incluirlo inmediatamente en la planificación de los siguientes turnos de patrulla.

## RF - 13: Registro documental de alta médica

El sistema debe permitir al Responsable de RRHH adjuntar y guardar un archivo (PDF o imagen) con el parte de alta médica oficial dentro del expediente del trabajador.