# Título (lee el source code del markdown para ver los comentarios)

Fecha de comienzo: 07 de Noviembre del 2022
Fecha de terminado: 

Autores:
 - @reynaldoverdugomacropay

## 1 TL;DR

<!--
párrafo corto que explica qué estas proponiendo
-->
Eligir el mejor framework para el desarrollo de API's para nodejs o typescript

## 2 Motivación

<!--
¿qué motiva esta decisión y por qué es importante?
el propósito de esta sección es articular de una manera sencilla el valor de la decision que vamos a tomar
-->
Nuestra empresa se encuentra en constante crecimiento en la creación de API's. Por lo tanto se debe elegir adecuadamente el framework para su desarrollo y así
obtener las siguientes ventajas:

  - Acorta los plazos de las entregas al mejorar los tiempos de productividad en el areá de Middleware.
  - No es necesario la creaciónn de una estrucuta desde cero.
  - Ahorro de tiempos en productividad al evitar escribir código repetitivo.
  - Facilita el mantenimiento del proyecto por lo que se vuelve de una manera más sencilla en el largo plazo, ya que dispone de una base estandarizada.
  - Buenas prácticas de desarrollo con el uso de patrones. 
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

Las propuestas para el uso de la documentación dentro de los proyectos en desarollo se encuentran: 
La propuesta del framework para la creación de API's se encuentra:
  - NestJs: Es un marco progresivo de NodeJs que crea aplicaciones dinámicas y escalables de nivel empresarial, al igual que ofrece una flexibilidad completa con el conjunto de extensas bibliotecas que contiene. 
  Su marco utiliza Typescript (un subconjunto de Javascript), es compatible y se adhiere a la arquitectura de código limpio mientras que conserva la complejidad del código de las aplicaciones a gran escala. Otro punto importante es que nos brinda una excelente integración con marcos de la misma familia como Fastify y Express.
  Nest nos puede potenciar doblemente la productividad de los desarrolladores y el rendimiento de las aplicaciones, esto es debe a la combinación de la programación reactiva orientada a objectos y funcional, por lo tanto nos ahorra un tiempo valioso.
    - Url: https://nestjs.com/

  La propuesta cuenta con varias Ventajas:
   -  El nivel de la curva de aprendizaje es baja 
   -  Arquitectura modular y por lo mismo permite utilizar otras bibliotecas de NodeJs.
   -  Cuenta con su propio CLI (Interfaz de linea de comandos)
   -  Una documentación exhaustiva.
   -  Se puede usar diferentes patrones arquitectónicos, pruebas unitarias sencillas y crear aplicaciones escalables. 
  
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
Para poder llevar acabo estas tarea de la documentación de aplicaciones tenemos diferentes alternativas que pueden cubrir las funciones que swagger realiza.

- Express: Express.js,también conocido como Express, encabeza la lista de los mejores marcos de Node.js. Tiene un enfoque minimalista y parece ser un marco clásico y sencillo para la arquitectura de codificación.
    - Url: https://raml.org/

- Fastify: Fastify es un framework inspirado en Hapi y Express que asegura ser super veloz, seguro y fácil de desarrollar ofreciendo un gran ecosistema de complementos.
    - Url: https://www.fastify.io/

- Koa: Uno de los marcos Node.js más dominantes, Koa hace maravillas al crear diferentes servicios web, también conocidos como API. Con Koa, crear estas API se vuelve súper divertido y fácil, ya que puede manejar de manera eficiente el middleware HTTP con un método similar a una pila.
    - Url: https://koajs.com/

- Hapi: Hapi es un servidor disponible comercialmente y un marco de código abierto para aplicaciones web . Es conocido por desarrollar servidores proxy, API REST y otras aplicaciones de escritorio, ya que el marco es confiable y rico en aspectos de seguridad. Tiene un lujoso conjunto de complementos integrados, por lo que no tiene que preocuparse por usar middleware no oficial.
    - Url: https://hapi.dev/


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


- Fastify:
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

- Comparacion de Precios


| Tipo   | De Paga? | Mensual  | Anual | Panel | Cloud? | Comentario |
| :---:  |  :---:  | :---: | :---:  |  :---:  | :---: | :---: |
| Swagger |    ✔    |  Planes de $90, $150, $300 USD  |   Planes de $75, $125, $250 USD  |   ✔   |    ✔   | Dependiendo del plan es la cantidad de Designers y Consumers y el mas completo para documentacion y facilidad de pruebas |
| RAML  |    ❌    |   Free   |   Free   |    ❌    |    ❌    | No cuenta con un panel administrativo de las api, codigo abierto|
| APIARY |   ❌ Obsoleto   |  Free  |   Free  |   ✔   |    ✔   | Esta gratuito pero esta limitado con muchas cosas|
| FASTAPI  |    ❌    |   Free   |   Free   |    ❌    |    ❌    | No cuenta con un panel administrativo de las api|



## 8 Preguntas sin resolver

<!--
¿ Qué preguntas no hemos resuelto?
-->
  - ¿Estamos dispuestos a manejar diferentes tipos de documentacion si se trata de aplicativos que sean incompatibles con la propuesta?
  - ¿Que sucedera con los proyectos previos?
  - ¿Se usara una misma estructura?
  - ¿Los desarrolladores estan dispuestos a tomar el riesgo de esta nueva implementacion?
  - ¿Que opinan de las propuestas?

## 9 Conclusión

