# Título (lee el source code del markdown para ver los comentarios)

Fecha de comienzo: 03 de Noviembre del 2022
Fecha de terminado: 

Autores:
 - @reynaldoverdugomacropay

## 1 TL;DR

<!--
párrafo corto que explica qué estas proponiendo
-->
Agregar en nuestras API's un framework|herramientas para documentarlas mediante una investigación.

## 2 Motivación

<!--
¿qué motiva esta decisión y por qué es importante?
el propósito de esta sección es articular de una manera sencilla el valor de la decision que vamos a tomar
-->

Nuestra empresa se encuentra en constante crecimiento creando o actualizando API's. Por lo tanto al documentarlas, tendremos las siguientes ventajas:

  - Entendimiento de cada una de nuestras API's.
  - Mejor toma de decisiones y ahorro de tiempos en productividad, ya que al conocer nuestras API's podemos re-utilizarlas siempre y cuando se de el caso.
  - Mejora de tiempos de productividad en el areá de Middleware, ya que cualquier pregunta, duda pueden consultar a la documentación del API.
  - Interfraz gráfica amigable para que las aréas externas puedan entender con facilidad. 

## 3 Propuesta de implementación

Actualmente se cuentan con templates para diferentes tipos de proyectos dependiendo del requerimiento y lenguaje o de la forma que se requiere el despliegue en aws.
  - Basado en eso templates de pueden modificar para incluir la documentacion con la api/libreria que se necesite dependiendo del caso.
  - Hay templates basados en lenguajes diferentes como lo son: NodeJs, Php, Java; Phyton, C#

Las propuestas para el uso de la documentación dentro de los proyectos en desarollo se encuentran: 
  - Swagger: Es una serie de reglas, herramientas y especificaciones que ayudan con la documentacion de las apis. Esta permite crear una documentacion bastante completa para que el resto de los integrantes del equipo puedan entenderla.
  Maneja una intefaz grafica que permite visualizar las apis asi como los comentarios y hacer pruebas para ver el funcionamiento de las mismas. Asi mismo muestra que mensajes puede mostrar en diversos tipos de caso.
   Ventajas:
   -  Es de las mas utilizadas
   -  Es compatible con node Js.
   -  La interfaz permite ver parte del codigo, asi como es muy amigable para el usuario
   - Permite ver los metodos de ingreso de datos y ver que recibe y que envia.

   Desventajas:
   - No es compatible con muchos lenguajes
   - Solo da 14 dias gratis de uso
   - Para tener mas colaboradores se debe ampliar el plan que se paga por mes
   Costos:
    Por Mes:
     -  $90 USD/Mes: 3 Designers/6 Consumers
     -  $150 USD/Mes: 5 Designers/10 Consumers
     -  $300 USD/Mes: 10 Designers/20 Consumers
    Por Año:
     -  $75 USD/Mes: 3 Designers/6 Consumers
     -  $125 USD/Mes: 5 Designers/10 Consumers
     -  $250 USD/Mes: 10 Designers/20 Consumers

  - RAML: Es parecido a Swagger, permitiendo y facilitando la documentacion de Api Rest de manera simplificada. Manteniendo la sincronizacion con la documentacion.
    Ventajas:
      - Proporciona documentacion interactiva.
      - compatible con Node Js y Php
      - Permite tener el control en la documentacion
    Desventajas:

  - Oracle+Apiary: Al igual que Swagger esta es una alternativa bastante llamativa, funciona de la misma manera, pero teniendo en cuenta que esta ligada con oracle. donde se pueden visualizar mas de un proyecto, y cuenta con conexion a github.
    Ventajas:
      - Conexion con github.
      - Permite el uso gratuito de manera ilimitada, pero esta restringido con ciertas caracteristicas.
      - Permite controlar quienes son colaboradores y quienes solo pueden visualiar
    Desventajas:
      - Actualmente la compra de planes es confuso.
      - Los planes de pago que manejaba estan obsoletos
      - Se tiene que comprar una suscripcion a Oracle Cloud
      - El modo gratuito solo permite 5 editores y 10 viewers
  - FastApi:


<!--
Este es el núcleo de tu propuesta, y su proposito es ayudarte a pensar en la solución. Esto debe ser un wireframe, no un documento perfecto con todos los detalles.

Escribir es pensar https://medium.learningbyshipping.com/writing-is-thinking-an-annotated-twitter-thread-2a75fe07fade

  - usa diagramas para ilustrat tus ideas o flujos
  - inluye ejemplos de código si estas proponiendo una interfaz o contrato de sistemsa nuevo
  - agrega links con las especificaciones de proyectos

El proposito de esta sección se resume en:
"Esta es la dirección en la que nos voy a llevar, alguién ve huecos en mi propuesta o tiene comentarios sobre cómo mejorarla?

 -->
 

## 4 Métricas

<!--
Que métricas debemos vamos a instrumentar, o monitorear para observar las implicaciónes de esta decisiòn?
Por ejemplo, cuando interactuamos con un sistema externo que tipo de latencia esperariamos o si agregamos una tabla nueva que tan rápido se llenaría?
-->

## 5 Riesgos e inconvenientes

<!--
¿Hay razones por las que no deberiamos hacer esto?
¿Qué riesgos estamos tomando? Por ejemplo, no tenemos experiencia con esta tecnología nueva o no entendemos la escala aún.
-->

## 6 Alternativas

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


## 8 Preguntas sin resolver

<!--
¿ Qué preguntas no hemos resuelto?
-->

## 9 Conclusión

