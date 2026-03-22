# 9. Definición de actores del sistema

A continuación, se definen los entes externos que interactúan con el sistema de GesSec S.L., divididos según su rol.

## Actores Principales (Humanos)

1. **Director General:** 
    * Usuario de nivel estratégico que utiliza el sistema desde la aplicación web en la central. Su objetivo principal es consultar cuadros de mando y obtener informes de rendimiento general, estadísticas de incidencias resueltas, tiempos de respuesta y urbanizaciones con mayor actividad.

2. **Jefe de Seguridad (Administrador):**
   * Usuario de nivel táctico y operativo. Es el encargado de planificar semanalmente los turnos, asignar vigilantes y vehículos a las patrullas, y consultar estadísticas detalladas del servicio. Además, actúa como administrador del sistema, configurando los permisos de acceso y las altas/bajas de los distintos perfiles de usuario.

3. **Operador de Central:**
   * Usuario que trabaja desde la aplicación web en la central de operaciones. Se encarga de la atención en primera línea: identifica a los residentes que llaman, crea y hace seguimiento de las incidencias, asigna alertas a los vigilantes más cercanos y gestiona los datos del padrón de residentes.

4. **Vigilante de Seguridad (Patrulla):**
   * Usuario de campo que interactúa exclusivamente a través de la aplicación móvil del sistema. Recibe notificaciones de incidencias, confirma la recepción de órdenes, reporta sus tiempos de desplazamiento, documenta la resolución de los problemas y puede autoasignarse incidencias.

5. **Responsable de Recursos Humanos (RRHH):**
   * Usuario de gestión de personal. Utiliza el sistema para mantener actualizados los datos personales y laborales de los empleados, registrar periodos de vacaciones o bajas, y recibir avisos automatizados cuando vayan a caducar las licencias de los vigilantes.

## Actores Secundarios (Sistemas Externos)

6. **Sistema de Alarmas (Viviendas y Perimetrales):**
   * Ente externo no humano que se comunica con el sistema central. Cuando los sensores detectan una anomalía, envía una alerta automática al sistema para que registre una incidencia, incluyendo identificadores y coordenadas GPS.

7. **Navegador GPS (Aplicación externa móvil):**
   * Sistema externo en el teléfono móvil del vigilante de seguridad. Actúa como actor de apoyo. El sistema de GesSec se comunica con él enviándole los datos de ubicación de una incidencia para que calcule y muestre la ruta óptima.

## Actores Pasivos

8. **Presidenta de la Comunidad / Residentes:**
   * **Descripción:** Actor pasivo que, aunque no interactúa directamente con el software operativo, está profundamente interesado en el resultado de los casos de uso (resolución rápida de incidencias). 
   * **Supuesto de diseño:** Se asume que el sistema generará y enviará de forma automatizada (vía email o SMS) notificaciones de estado sobre las incidencias reportadas y un informe resumen mensual para el Presidente justificando así su inclusión como actor pasivo del sistema.