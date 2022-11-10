# Título (lee el source code del markdown para ver los comentarios)

Fecha de comienzo: 07 de Noviembre del 2022
Fecha de terminado: 

Autores:
 - @reynaldoverdugomacropay

## 1 TL;DR

<!--
párrafo corto que explica qué estas proponiendo
-->
Eligir el mejor framework para el desarrollo de API's para nodejs.

## 2 Motivación

<!--
¿qué motiva esta decisión y por qué es importante?
el propósito de esta sección es articular de una manera sencilla el valor de la decision que vamos a tomar
-->
Nuestra empresa se encuentra en constante crecimiento en la creación de API's. Por lo tanto se debe elegir adecuadamente el framework para su desarrollo y así obtener las siguientes ventajas:

  - Acorta los plazos de las entregas al mejorar los tiempos de productividad en el areá de Middleware.
  - No es necesario la creaciónn de una estrucuta desde cero.
  - Ahorro de tiempos en productividad al evitar escribir código repetitivo.
  - Facilita el mantenimiento del proyecto por lo que se vuelve de una manera más sencilla en el largo plazo, ya que dispone de una base estandarizada.
  - Buenas prácticas de desarrollo con el uso de patrones como lo son el patron de inyección de dependecias y repository.
  - Altamente configurable con ORM's y patrones de este tipo como lo son Active Record y Data Mapper.
  - Facilita la colaboración con otros desarrolladores.

## 3 Propuesta de implementación

<!--
Este es el núcleo de tu propuesta, y su proposito es ayudarte a pensar en la solución. Esto debe ser un wireframe, no un documento perfecto con todos los detalles.

Escribir es pensar https://medium.learningbyshipping.com/writing-is-thinking-an-annotated-twitter-thread-2a75fe07fade

  - usa diagramas para ilustrat tus ideas o flujos
  - inluye ejemplos de código si estas proponiendo una interfaz o contrato de sistemsa nuevo
  - agrega links con las especificaciones de proyectos

El proposito de esta sección se resume en:
"Esta es la dirección en la que nos voy a llevar, alguién ve huecos en mi propuesta o tiene comentarios sobre cómo mejorarla?

 -->
Actualmente en el departamento de middlewares, en la elaboración de API's, se utilizan diferentes tipos de frameworks para su creación y otros ya existentes que se les da un mantimiento. Estos pueden estar desarrollados por los siguientes lenguajes segun las especificaciones que se requiera, por ejemplo: NodeJs, Php, Java, Phyton, C#. El motivo es unificar la creación de API's a un framework y así lograr una mejora en el tiempo de desarrollo como en la estructura del código, optimizando el area de middlewares.

La propuesta del framework para la creación de API's se encuentra:
  - NestJs: Es un marco progresivo de NodeJs que crea aplicaciones dinámicas y escalables de nivel empresarial, al igual que ofrece una flexibilidad completa con el conjunto de extensas bibliotecas que contiene. 
  Su marco utiliza Typescript (un subconjunto de Javascript), es compatible y se adhiere a la arquitectura de código limpio mientras que conserva la complejidad del código de las aplicaciones a gran escala. Otro punto importante es que nos brinda una excelente integración con marcos de la misma familia como Fastify y Express.
  Nest nos puede potenciar doblemente la productividad de los desarrolladores y el rendimiento de las aplicaciones, esto es debe a la combinación de la programación reactiva orientada a objectos y funcional, por lo tanto nos ahorra un tiempo valioso.
    - Url: https://nestjs.com/

  La propuesta cuenta con varias Ventajas:
   -  Arquitectura modular y por lo mismo permite utilizar otras bibliotecas de NodeJs.
   -  Cuenta con su propio CLI (Interfaz de linea de comandos).
   -  Una documentación exhaustiva.
   -  Se puede usar diferentes patrones arquitectónicos, pruebas unitarias sencillas y crear aplicaciones escalables.
   -  Puedes construir servicios backend que van desde API RESTful, aplicaciones GraphQL, aplicaciones MVC, Web sockets, CLI.
   -  Inicio rapido, mientras los desarrolladores se enfocan en la lógica, el marco se encarga de otros aspectos importantes como la seguridad.

  Usabilidad:
    Creación y despliegue de aplicaciones comprobables, escalables, poco acopladas y fáciles de mantener a nivel empresarial.
  
  Seguridad del framework propuesto:
  Nestjs proporciona la mayoría de enfoques y estrategias de seguridad, como lo son la autenticación, autorización, encriptación, hashing, CSRF, entre otros. Apoyado y basado en la famosa librería passport. 
    - La autenticación es una parte esencial de la mayoría de las aplicaciones. Passport es la biblioteca de autenticación de node.js más popular, conocida por la comunidad y utilizada con éxito en muchas aplicaciones de producción. Passport ejecuta una serie de pasos para:
      - Autenticar a un usuario verificando sus "credenciales" (como nombre de usuario/contraseña, JSON Web Token ( JWT ) o token de identidad de un proveedor de identidad).
      - Administrar el estado autenticado (mediante la emisión de un token portátil, como un JWT, o la creación de una sesión Express ).
      - Adjunte información sobre el usuario autenticado al Requestobjeto para su uso posterior en los controladores de ruta.
    - La autorización se refiere al proceso que determina lo que un usuario puede hacer. Por ejemplo, un usuario administrativo puede crear, editar y eliminar publicaciones. Un usuario no administrativo solo está autorizado para leer las publicaciones.
      - Implementación básica de RBAC; el control de acceso basado en roles ( RBAC ) es un mecanismo de control de acceso independiente de la política definido en torno a roles y privilegios. En esta sección, demostraremos cómo implementar un mecanismo RBAC muy básico con Nest Guards.
    - Hashing es el proceso de convertir una clave dada en otro valor. Se utiliza una función hash para generar el nuevo valor de acuerdo con un algoritmo matemático. Una vez que se ha realizado el hashing, debería ser imposible pasar de la salida a la entrada.
    
  
## 4 Métricas

<!--
Que métricas debemos vamos a instrumentar, o monitorear para observar las implicaciónes de esta decisiòn?
Por ejemplo, cuando interactuamos con un sistema externo que tipo de latencia esperariamos o si agregamos una tabla nueva que tan rápido se llenaría?
-->

En estos momentos existen varios inconvenientes graves en el desarrollo de aplicativos para API's segun los requermientos pueden estar hechos en diferentes lenguajes, la opción de centralizar dichos proyectos llevaría más tiempo del que se dispone cada proyecto. Por lo tanto, la propuesta de centralizar en un solo tipo de lenguaje y framework se vería beneficiada para los aplicativos nuevos en los cuales tengan el proposito de desarrollar API's, ya que al ser desarrollados desde un solo framework o marco, facilitaría mucho la compresión de los proyectos y de esta menera evitar tiempo de más al tratar de comprender varios frameworks o lenguajes. Por mientras que los que ya estan en produccion se podrian mantener como estan hasta que se les permita hacer un rediseño, adaptandolo a las nuevas tecnologias que se estan implementando y al marco de trabajo. 

En la mayoría de los proyectos ya realizados y que van estar antes del cambio realizado por la empresa, presentan un tiempo de respuesta significativamente lente, aunque nos referimos a los proyectos grandes que ya están siendo usados por el usuario final, por lo tanto, no conveniente hacer una rediseño por el momento. De esta menera la propuesta quedara solo para los aplicativos que ya cuenten con el marco de trabajo actual, nuevos o recientes. 

## 5 Riesgos e inconvenientes

<!--
¿Hay razones por las que no deberiamos hacer esto?
¿Qué riesgos estamos tomando? Por ejemplo, no tenemos experiencia con esta tecnología nueva o no entendemos la escala aún.
-->
A su vez la propuesta con ciertas desventajas:

- Es difícil para desarrolladores que están comenzando a programar por primera vez
- Al tener una estructura muy definida puede llegar a confundir a los que ingresan a un proyecto hecho por Nest por primera vez, esto suele sucede cuando se navega por los diferentes archivos del proyecto.
- Esta inspirado en Angular, aunque esto sea conveniente para desarrolladores que han llegado a ver Angular, para los que no lo han visto llega a ser abrumador y confuso
- Un cambio grande en la manera de manejar los proyectos
- Hay proyectos ya hechos y que se encuentran en produccion que hacerles cambio requeriria hacer despliegues nuevamente.


## 6 Alternativas
Para poder realizar el desarrollo de API's, por medio de un framework, tenemos diferentes alternativas contempladas que pueden cubrir algunas funcionalidades necesarias que realiza NestJS.

- Express: Express.js,también conocido como Express, encabeza la lista de los mejores marcos de Node.js. Tiene un enfoque minimalista y parece ser un marco clásico y sencillo para la arquitectura de codificación.
    - Url: https://raml.org/

- Fastify: Fastify es un framework inspirado en Hapi y Express que asegura ser super veloz, seguro y fácil de desarrollar ofreciendo un gran ecosistema de complementos.
    - Url: https://www.fastify.io/

- Koa: Uno de los marcos Node.js más dominantes, Koa hace maravillas al crear diferentes servicios web, también conocidos como API. Con Koa, crear estas API se vuelve súper divertido y fácil, ya que puede manejar de manera eficiente el middleware HTTP con un método similar a una pila.
    - Url: https://koajs.com/

- Hapi: Hapi es un servidor disponible comercialmente y un marco de código abierto para aplicaciones web . Es conocido por desarrollar servidores proxy, API REST y otras aplicaciones de escritorio, ya que el marco es confiable y rico en aspectos de seguridad. Tiene un lujoso conjunto de complementos integrados, por lo que no tiene que preocuparse por usar middleware no oficial.
    - Url: https://hapi.dev/

Igual podemos tomar como alternativa uno de los frameworks más influyentes al momento de crear API's utilizando Python:

- FastAPI es un framework para construir APIs de forma sencilla y rápida con Python que en los últimos tiempos se ha vuelto muy popular. Actualmente es considerado como uno de los frameworks basados en Python más rápidos y, además,  proporciona también una gran velocidad a la hora de abordar el desarrollo de una API al incorporar, entre otras cosas, validación de datos y de documentación de forma automática, lo cual lo convierte en un candidato ideal para realizar el backend de cualquier aplicación web.
    - Url: https://fastapi.tiangolo.com/es/



<!--
¿Hay otras formas de resolver éste problema?
-->

## 7 Impacto potencial y dependencias

<!--
  ¿Qué otros sistemas se verán afectados con esta propuesta?
  ¿Qué consideraciones de seguridad debemos tener?¿Como pueden explotar esta parte del sistema?
  ¿Que impacto tiene esta decision sobre soporte al cliente?

  Aquí buscamos ser concientes del ambiente en el que operamos y generar empatía hacia otros que pueden verse afectados por nuestra decisión.
 -->

- Express:
    - Ventajas:
        - Proporciona una documentacion exhaustivo.
        - Análisis del cuerpo de las peticiones HTTP.
        - Análisis de las cookies.
        - Determinación de las cabeceras apropiadas para las respuestas.
        - Cabeceras automáticas en las respuestas.
        - Enrutado y mejor organización del código
        - Identificación, validación sesiones.
        - Patrón arquitectónico MVC
        - Alto rendimiento: varias operaciones se ejecutan de forma independiente entre sí mediante programación asíncrona
        - Paquetes de programación rápidos del lado del servidor: el marco tiene muchas características de Node.js como funciones y acelera el proceso con pocas líneas de código. 

    - Desventajas:
        - No cuenta con generadores de modelos, por lo tanto con lleva más tiempo en el desarrollo.
        - Estrictamente para el lenguaje de programación JavaScript.
        - No es un framework progresivo y por lo tanto no tiene las funciones principales al inciar un poryecto desde cero.
    
    - Usabilidad: Se puede desarrollar aplicaciones web más rápido con el marco, ya que tiene bases casi disponibles para la generación de API. Puede usarlo para cualquier aplicación de nivel empresarial o basada en navegador debido a su sólido enrutamiento, plantillas, funciones de seguridad y disposiciones de manejo de errores.  

    - Seguridad: N/A


- Fastify:
    - Ventajas:
        - Alto rendimiento, dependiendo de la complejidad del código, puede atender hasta 30 mil solicitudes por segundo.
        - Basado en esquemas, aunque no es obligatorio, se recomienda JSON para la validación de rutas y serializar salidas, internamente es copilado en una función de alto rendimiento.
        - Preparado para usarse con Typescript
        - Fácil de usar para desarrolladores, el marco está diseñado para ser muy expresivo y para ayudar a los desarrolladores en su uso diario, sin sacrificar el rendimiento ni la seguridad.
    - Desventajas:
      - No cuenta con una documentación tan exhaustivo.
      - Por la similitud, los desarroladores prefieren hacer uso de express que fastify.
      - El apoyo de la comunidad es regular. 
      - Existe incompatibilidad con algunas librerias. 

    - Usabilidad:
    Es un marco web para Node.js centrado en el rendimiento y la sobrecarga baja , lo que lo convierte en una excelente opción para quienes están desarrollando una arquitectura basada en microservicios.

    - Seguridad: N/A

- Koa:
    - Ventajas:
        - Maneja los errores excepcionalmente 
        - Es un marco personalizable y futurista: se conoce como una versión ligera de Express
        - Tiene middleware en cascada (Personalizar la experiencia del usuario)
        - Normaliza las inconsistencias de los nodos y ayuda a mantener el código
        - Tiene más opciones de personalización; permite crear aplicaciones desde cero

    - Desventajas:
        - No cuenta con generadores de modelos, por lo tanto con lleva más tiempo en el desarrollo.
        - Estrictamente para el lenguaje de programación JavaScript.
        - No es un framework progresivo y por lo tanto no tiene las funciones principales al inciar un poryecto desde cero.

    - Usabilidad: 
    Cuando el rendimiento es una demanda crítica de su aplicación web, Koa es lo que necesita. Especialmente para un gran proyecto, el marco puede crear aplicaciones extensas con equipos de desarrollo grandes y experimentados. Bajo ciertas circunstancias, Koa ha demostrado ser un marco más rápido que Express. 

    - Seguridad: N/A

- Hapi:
    - Ventajas:
        - Aplicaciones escalables
        - Valores predeterminados seguros
        - Corrección de errores rápida y fácil
        - Compatible con API Rest y aplicaciones de proxy HTTPS
        - Almacenamiento en caché predeterminado, autenticación y validación de entrada

    - Desventajas:
        - No cuenta con generadores de modelos, por lo tanto con lleva más tiempo en el desarrollo.
        - Estrictamente para el lenguaje de programación JavaScript.
        - No es un framework progresivo y por lo tanto no tiene las funciones principales al inciar un poryecto desde cero.

    - Usabilidad: 
    Hapi.js funciona de maravilla en el desarrollo de aplicaciones de redes sociales más seguras, escalables y en tiempo real. Los desarrolladores lo usan principalmente para construir proxies y servidores API. 

    - Seguridad:
       - Valores predeterminados seguros, actualizados regularmente; protege la carga del servidor con límites de carga útil y tiempos de espera de solicitud, igualemnte bloquea los mensajes de error que podrían filtrar información o hacer eco de las vulnerabilidades.
       - Higiene de código de extremo a extremo; hapi requiere la configuración más segura para administrar, controlar y distribuir código, incluido 2FA para todos los colaboradores.
       - Arquitectura integrada de autorización y autenticación; la API de autorización y autenticación más completa disponible en un marco de Node.
       - Funciones avanzadas; con cookies cifradas y firmadas, rotación de secretos o claves y encabezados de seguridad HTTP, no hay excusas para crear aplicaciones inseguras.
       - Propiedad confiable y predecible; cuando algo sale mal, sabe a quién contactar. Las actualizaciones de seguridad se manejan bajo un protocolo estricto y bien definido.
       - Ecosistema enriquecido; el amplio conjunto de complementos oficiales de hapi significa que ya no tendrá que confiar ciegamente en algún middleware que haya encontrado para una funcionalidad crítica solo porque tiene una gran cantidad de npm.
       - Experiencia en seguridad interna; creada por Eran Hammer, el autor de las especificaciones de OAuth y otros protocolos de identidad.

- FastApi:
  - Ventajas: 
    - Compatibilidad con async/await. Con FastAPI puede escribir código asincrónico listo para usar. Una característica de bienvenida al ecosistema del marco de trabajo de Python que suele ser de naturaleza síncrona.
    - Tiene configuraciones por defecto razonables para todo, con configuraciones opcionales en todas partes.
    - FastAPI está basado y es completamente compatible con Starlette (conjunto de herramientas que es ideal para crear servicios web asíncronos). Tanto así, que cualquier código de Starlette que tengas también funcionará.
    - Gran variedad en validaciones, por ejemplos (json, list, texto, números, URL, email, entre otros).
    - Genera su propia documentación con swagger para API's
  - Desventajas:
    - Información externa minima. Dado que FastAPI es un marco relativamente nuevo, la comunidad es relativamente menor al framework propuesto.

  - Usabilidad:
  FastApi se usa para la creación de API's al ser un framweork de alto rendimiento, aumentando su rapidez, intuición, basado en estanderes, entre otras características primordiales al crear API's.

  - Seguridad: La seguridad y la autenticación están integradas. Sin ningún compromiso con bases de datos ni modelos de datos. Al igual que todos los esquemas de seguridad están definidos en OpenAPI incluyendo, HTTP basic, OAuth2 y JWT tokens, API Keys, más todos las características de seguridad de Starlette (incluyendo sesiones de cookies)

- Comparación de Precios

Tabla comparativa de frameworks
| Framework | Rendimiento | Soporte en lambdas  | Seguridad | Curva de aprendizaje | Documentación exhaustiva | Progresivo | Agíl desarrollo | Documentación automatica integrada para el consumo de API's | Escalabilidad |
| :---:  |  :---:  | :---: | :---:  |  :---:  | :---: | :---: | :---: | :---: | :---: |
| NestJs |   ✔    |   ✔   |   ✔   |   alta   |   ✔   |   ✔   |   Medio   |   ❌   |   ✔   |
| ExpressJs |   ❌   |   ✔   |   ❌   |   Baja   |   ❌   |   ❌   |   Agíl   |   ❌   |   ❌   |
| KoaJs |   ❌   |   ✔   |   ❌   |   Baja   |   ❌   |   ❌   |   Agíl   |   ❌   |   ❌   |
| FastifyJs |   ✔   |   ✔   |   ❌   |   Baja   |   ✔   |   ❌   |   Agíl   |   ❌   |   ❌   |
| HapiJS |   ❌   |   ✔   |   ✔   |   Baja   |   ✔   |   ❌   |   Agíl   |   ❌   |   ✔   |
| FASTAPI  |   ✔   |   ✔   |   ✔   |   Baja   |   ✔   |   ❌   |   Agíl   |   ✔(Swagger)   |   ❌   |

## 8 Preguntas sin resolver

<!--
¿ Qué preguntas no hemos resuelto?
-->

## 9 Conclusión

