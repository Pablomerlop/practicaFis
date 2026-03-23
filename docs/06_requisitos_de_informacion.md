# 6. Requisitos de información

## RI - 01: Empleados

El sistema debe almacenar la información de todos los empleados (vigilantes y personal de central), incluyendo:

1- Datos personales: nombre completo, fecha de nacimiento, DNI, domicilio y teléfonos de contacto.  
2- Datos laborales: fecha de alta en la empresa, categoría profesional, el turno de preferencia para ser asignado y estado de la habilitación profesional (fecha de caducidad).  
3- Situación actual: activo, de baja (médica o de cualquier otro tipo), vacaciones o excedencia.

## RI - 02: Vehículos

El sistema debe almacenar la siguiente información de cada vehículo:

1- Identificación: matrícula, marca, modelo y año de compra.  
2- Uso y kilometraje: kilómetros totales recorridos y el registro de kilómetros al inicio y al finalizar cada turno (apuntados por el vigilante).  
3- Disponibilidad: estado actual del vehículo para evitar conflictos en la asignación de patrullas.  

## RI - 03: Residentes

El sistema debe almacenar la siguiente información de cada residente:

1- Identificación: nombre completo y DNI o NIE.  
2- Ubicación: Urbanización a la que pertenece y dirección completa de la vivienda.  
3- Contacto: Lista de números asociados a la vivienda (fijos y móviles).

## RI - 04: Incidencias

El sistema debe almacenar la siguiente información de cada incidencia:

1- Datos de apertura: identificación del informante (residente identificado o datos de quien llama si es externo), urbanización y dirección donde ocurre el incidente, tipo de incidencia (alarma de intrusión activada, alarma de humo, accidente, problema de causa natural, solicitud de asistencia general u otro), descripción libre del problema contado por el residente y la fecha y hora.  
2- Gestión y respuesta: vigilante asignado (su identificación), registro de la confirmación de recepción y horas de salida y llegada al lugar.  
3- Resolución y cierre: tipo definitivo del incidente, descripción de lo que encontró, solución adoptada y hora de resolución.  

## RI - 05: Urbanizaciones

El sistema debe almacenar la siguiente información de las comunidades de propietarios gestionadas:

1- Identificación y características: nombre de la urbanizacion, dimensiones y características particulares (si es tranquila, si tiene mucho movimiento, si es muy cerrada...)  
2- Datos del contrato: número de patrullas semanales y tiempos de respuesta comprometidos ante incidencias.  
3- Alarmas de zonas comunes: listado de las alarmas instaladas en el perímetro o zonas compartidas (vallas, club social, entrada), incluyendo su identificador, el lugar donde están y sus coordenadas GPS.





