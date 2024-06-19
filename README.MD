# differences between monorepo and multirepo

# Multirepo (Multiple Repositories)
Estructura:

Cada proyecto o componente tiene su propio repositorio independiente.
Ejemplo: Un repositorio para el frontend, otro para el backend, otro para la base de datos, etc.
Ventajas: 

Aislamiento: Cambios en un repositorio no afectan directamente a otros, lo que facilita el aislamiento de problemas.
Permisos: Es más sencillo gestionar permisos de acceso específicos para cada repositorio.
Historial: El historial de cambios es más claro y específico para cada proyecto.
Desventajas:

Coordinación: Puede ser complicado coordinar cambios entre varios repositorios, especialmente si hay dependencias fuertes entre ellos.
Mantenimiento: La gestión de múltiples repositorios puede ser tediosa y requerir más esfuerzo en términos de configuración y administración.
Dependencias: Las dependencias entre proyectos pueden ser difíciles de manejar y versionar correctamente.




# Monorepo (Monolithic Repository)
Estructura:

Todos los proyectos o componentes se almacenan en un único repositorio compartido.
Ejemplo: El frontend, backend, y otros componentes residen en diferentes directorios dentro del mismo repositorio.
Ventajas:

Sincronización: Es más fácil realizar cambios sincronizados en múltiples proyectos, ya que todos están en el mismo repositorio.
Consistencia: Las herramientas y librerías compartidas pueden ser gestionadas de forma más consistente.
Visibilidad: Los desarrolladores tienen visibilidad completa de todo el código, facilitando la comprensión y colaboración entre equipos.
Desventajas:

Escalabilidad: A medida que el repositorio crece, puede volverse lento y difícil de manejar.
Conflictos: La alta cantidad de cambios puede incrementar la probabilidad de conflictos de código.
Permisos: Gestionar permisos puede ser más complejo, ya que todos tienen acceso a todo el repositorio.


# Ejemplos del Mundo Real
Multirepo: Es utilizado por empresas que prefieren una mayor separación entre sus componentes y proyectos, como muchas organizaciones que siguen el enfoque de microservicios.
Monorepo: Es usado por grandes empresas tecnológicas como Google, Facebook y Microsoft, quienes tienen infraestructura y herramientas avanzadas para manejar grandes cantidades de código en un único repositorio.

# Decisión
La elección entre multirepo y monorepo depende de varios factores, incluyendo:

Tamaño del equipo: Equipos grandes con muchas dependencias pueden preferir un monorepo.
Infraestructura: La disponibilidad de herramientas y la infraestructura para gestionar un monorepo de gran tamaño.
Estrategia de desarrollo: La arquitectura del software y cómo se gestionan las dependencias y los ciclos de lanzamiento.


# Que son los métodos http (Put, Post, Pat)


también conocidos como verbos HTTP, son instrucciones que indican la acción que se desea realizar sobre un recurso específico en un servidor web. Son fundamentales para la comunicación entre un cliente y un servidor web

Entre los métodos HTTP más comunes se encuentran GET, POST, PUT y DELETE
## GET: Recupera datos de un recurso.
## POST: Envía datos al servidor para su procesamiento o almacenamiento.
## PUT: Actualiza un recurso existente.
## DELETE: Elimina un recurso.


# Métodos HTTP adicionales:

•	PATCH: Similar a PUT, pero actualiza solo una parte específica de un recurso
•	HEAD: Similar a GET, pero solo recupera los encabezados de la respuesta, no el cuerpo del recurso.
•	OPTIONS: Obtiene las opciones de solicitud HTTP disponibles para un recurso específico.




# VERSIONAMIENTO QUE USAREMOS DE NODE


•	Utilizaremos para este proyecto la versión v20.14.0 ya que es la versión con soporte a largo plazo (lts) en este momento

# ¿Vamos a utilizar multirepo o monorepo?

En este caso vamos a utilizar multirepo ya que hemos visto que los cambios en un repositorio no afectan directamente a otros, lo que facilita el aislamiento de problemas  y es más sencillo gestionar permisos de acceso específicos para cada repositorio.

# ¿Problemas, objetivos y/o servicios del proyecto o unidades residenciales?
para ver el alcance del projecto 
  Requerimientos por parte de los usuarios o dueños de apartamentos o persona que viven en la unidad
- es necesario poder tener cuenta de usuario por cada apartamento
- que puedan hacer solicitud de reservas de zonas comunes
- que puedan enviar fotos y/o emails con problemas de daños o situaciones en el conjunto
- un enlace para el pago de la factura de la administracion


  Requerimientos por parte de la administracion
- usuario admin
- poder hacer publicaciones y/o avisos
- poder enviar cartas a correos certificados de los usuarios para notificaciones
- poder crear encuestas en la pagina sobre diferentes temas
- tener un apartado de gestion del edficio economicamente.
- hacer la aprobacion de las reservas de zonas comunes.


# differences between npm and yarn


Tanto NPM como Yarn son herramientas potentes para la gestión de paquetes de JavaScript y la elección entre ellas depende de los requisitos y preferencias de su proyecto. NPM, al ser el administrador de paquetes predeterminado para Node.js, goza de una adopción y compatibilidad generalizadas. Por otro lado, Yarn ofrece ventajas como rendimiento mejorado, resolución de dependencia determinista, instalación paralela y mejor soporte para espacios de trabajo y monorepos.


# Definition of nvm

Node Version Manager (NVM), como su nombre lo indica, es una herramienta para administrar las versiones de Node en su dispositivo . Es posible que diferentes proyectos en su dispositivo utilicen diferentes versiones de Node. Es posible que usar solo una versión (la instalada por npm) para estos diferentes proyectos no le brinde resultados de ejecución precisos.

basicamente es para poder saltar de version node.js y hacer un update rapido 

(pagina para instalar nvm paso a paso https://4geeks.com/es/how-to/como-instalar-nvm-en-windows)


# Definiton of swagger

Conjunto de herramientas Swagger:

Es un conjunto de herramientas de código abierto que se basan en la especificación OpenAPI.

Incluye herramientas para:
- Documentar APIs: Genera documentación completa y legible para humanos y máquinas a partir de la definición de la API.
- Diseñar APIs: Permite a los desarrolladores diseñar APIs de forma visual y colaborativa.
- Probar APIs: Proporciona herramientas para probar las APIs y garantizar su correcto funcionamiento.
- Generar código: Puede generar código fuente en diferentes lenguajes de programación a partir de la definición de la API.


En resumen, Swagger es una herramienta esencial para el desarrollo y consumo de API REST.



# definition of Eslint

ESLint es una herramienta de análisis estático de código para JavaScript.

Su función principal es identificar y corregir errores, problemas de estilo y violaciones de las convenciones de codificación en proyectos de desarrollo de JavaScript.

ESLint ayuda a los desarrolladores a escribir código más limpio, consistente y mantenible.

Es una herramienta muy versátil que se puede configurar para adaptarse a las necesidades de cualquier proyecto o equipo de desarrollo.

