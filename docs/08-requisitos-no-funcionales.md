### 8. Requisitos No Funcionales (Modelo FURPS+ y Sommerville)

A continuación se detallan los requisitos que definen cómo debe comportarse el sistema (su calidad y restricciones), organizados según la clasificación FURPS+ y las categorías de Sommerville, utilizando un lenguaje claro:

#### Usabilidad (Usability)
* **Interfaz móvil intuitiva:** La aplicación para los vigilantes debe ser muy fácil de usar, con una pantalla clara, botones grandes y sin menús complicados, pensando en los usuarios que no tienen facilidad con la tecnología.
* **Plataforma móvil:** La app de los vigilantes debe estar diseñada preferiblemente para teléfonos android, ya que son los dispositivos de empresa actuales.
* **Acceso web en central:** El sistema para los operadores de la central debe ser una página web, para evitar tener que instalar programas especiales en los ordenadores de la oficina.

#### Fiabilidad (Reliability)
* **Tolerancia a baja cobertura:** La aplicación móvil debe ser capaz de funcionar correctamente, o al menos mantener sus funciones básicas, en zonas de las urbanizaciones donde la señal de internet sea débil o inexistente.

#### Rendimiento (Performance)
* **Alertas de tiempo crítico:** El sistema debe ser capaz de controlar el tiempo en tiempo real y lanzar un aviso automático a la central si un vigilante tarda más de dos minutos en responder a una alerta.

#### Soporte y Mantenibilidad (Supportability)
* **Mantenimiento centralizado:** Gracias al uso de una aplicación web en la central, las actualizaciones del sistema se aplicarán directamente sin necesidad de intervenir equipo por equipo.

#### Requisitos "+" (Seguridad, Interoperabilidad y Legales - Sommerville)
* **Seguridad y Privacidad (Control de acceso):** El sistema debe garantizar que cada empleado vea solo lo necesario para su trabajo. Se deben crear roles estrictos (Dirección, Jefe de Seguridad, Operador, Vigilante y RRHH) para proteger la información.
* **Interoperabilidad (Integración con mapas):** La aplicación móvil debe poder conectarse de forma fluida con el navegador GPS del propio teléfono para guiar rápidamente al vigilante hasta el lugar de la incidencia.
* **Requisitos Legales / Normativos:** El sistema debe tener en cuenta las leyes de seguridad privada, incluyendo una función obligatoria que controle la vigencia de las habilitaciones profesionales de los vigilantes.