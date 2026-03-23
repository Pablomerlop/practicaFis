# 7. Reglas de negocio

## RN - 01: Habilitación personal

Todo vigilante de seguridad debe de poseer una habilitación profesional en vigor para poder realizar cualquier actividad operativa. 
El sistema no permitirá la asignación de un vigilante a un turno de patrulla o a una incidencia si su fecha de caducidad de la habilitación es anterior o igual a la fecha del servicio.

## RN - 02: Control de Kilometraje por Turno

La empresa exige un control estricto del uso de los vehículos para el mantenimiento preventivo y el control de costes. 
El sistema no permitirá finalizar la hoja de turno de un vigilante si no se han introducido los kilómetros totales del vehículo al cierre de la patrulla. Además, el kilometraje de cierre debe ser igual o superior al kilometraje registrado en la apertura del mismo turno.

## RN - 03: Operatividad de Vehículos

Garantizar que los vigilantes solo utilicen vehículos que estén en condiciones seguras y que la central no asigne recursos que no están disponibles físicamente.
El sistema bloqueará la posibilidad de asignar un vehículo a un turno de patrulla o a una incidencia si su estado actual es diferente a "Operativo" (por ejemplo, si está marcado como "Averiado", "En taller" o "Siniestro").

## RN - 04: Identificación Automática de Intervinientes

Optimizar la apertura de incidencias y garantizar que la información de contacto es veraz y pertenece a la base de datos de clientes.
El sistema solo realizará la identificación automática del residente (mostrando su nombre, dirección y urbanización) si el número de teléfono de la llamada entrante coincide con alguno de los números registrados y vinculados a una vivienda en el RI-03 (Residentes). En caso contrario, el sistema obligará a la apertura de una "Ficha de Informante Externo" para el registro manual de datos.

## RN - 05: Control de respuestas a alertas

Asegurar que los avisos se atiendan rápido y que ninguna emergencia se quede sin respuesta por un descuido.
El sistema controlará cuánto tarda un vigilante en aceptar un aviso en su móvil. Si pasan más de 2 minutos sin que el vigilante confirme que lo ha recibido, el sistema enviará una alerta automática a la central para que el operador pueda pasarle el trabajo a otro compañero disponible de inmediato.
