---
title: "Evaluación de una Arquitectura Software por medio de ATAM"
author: [ ]
date: "2019"
subtitle: "Segunda Práctica de Arquitectura de Software - UPM"
logo: capturas/logo.png
titlepage: "true"
toc: "true"
toc-own-page: "true"
lof : "true"
lof-own-page: "true"
lot: "true"
lot-own-page: "true"
listings-no-page-break: "true"
...

# 1. Introducción
> Posible cita aquí




## 1.1 Propósito del documento

Documento realizado por:

- Luis Mata Aguilar
- Carlos Gómez Robles
- Daniel Rodríguez Manzanero
- Yeray Granada Layos
- María Gallego Martín
- Alejandro de la Fuente Perdiguero
 
El propósito de este documento es evaluar la arquitetura software recogida en el documento "a_evaluar.pdf" del repositorio de GitHub [lmataa/ehealth-eval-doc](https://github.com/lmataa/ehealth-eval-doc). El cual corresponde al resultado de la primera práctica de la asignatura de Arquitectura y Diseño SW del grupo GIWM31 redactado por:
  

- Pérez Souza, Miguel Ángel
- Romero Andrés, Eric
- Sastre Gallardo, Alberto
- Torres Sánchez, Alfonso
- Vila Marin, Carlos

El documento está dirigido a un conjunto de stakeholders de dicho proyecto, entre los que destacan sobre los demás *"Project decision makers"*, o responsables de la toma de decisiones del proyecto, así como los stakeholders referentes a la arquitectura, responsables de gestionar atributos de caldiad que la arquitectura debe cumplir.


## 1.2 Definiciones, Acrónimos y Abreviaturas

En esta sección se incluye:

- Definiciones de términos usados en este documento requeridos para la correcta interpretación de las construcciones lingüisticas empleadas.
- Acrónimos utilizados en el documento relacionados con el dominio del problema.
- Abreviaturas utilizadas a lo largo del documento.

### 1.2.1 Definiciones

- **Atributos de calidad**: 
- **Business Goals**:
- **Business Drivers**:
- **ATAM**: 
- **Riesgo**:  
- **No riesgo**: 


### 1.2.2 Acrónimos y Abreviaturas

- **NDA**: Non-disclosure agreement, acuerdo de confidencialidad
- **a2**:
- **a3**:
- **a4**:

## 1.3 Referencias

En esta sección se incluyen todas las referencias bibliográficas consultadas para la elaboración de este documento.

Citation | Table
---------|-------
Author   | Document

Table: Referencias

## 1.4 Estructura del documento

El presente documento se ha organizado como sigue:

- **Capítulo 1**: se realiza una introducción que incluye el propósito del documento, definiciones, acrónimos, y abreviaturas utilizados así como las referencias bibliográficas consultadas.

- **Capítulo 2**: memoria del desarrollo la fase 0 del proceso ATAM referente a la validación de una arquitectura software.

- **Capítulo 3**: memoria del desarrollo de la fase 1 del proceso ATAM referente al análisis de business goals, business drivers, patrones arquitectónicos, atributos de calidad, etc.

- **Capítulo 4**: artefacto de análisis de los escenarios existentes así como la identificación de nuevos escenarios.

- **Capítulo 5**: corresponde a la fase 3 del proceso ATAM, follow up, queda introducida pero está fuera del alcance de este documento.

- **Capítulo 6**: principales conclusiones del trabajo de evaluación.

- **Capítulo 7**: anexo 1 con el acta de reuniones.

- **Capítulo 8**: anexo 2 con el NDA firmado por las partes.


# 2. Fase 0: Preparación

En esta fase de la evaluación ATAM, se le da comienzo al proceso de evaluación. En primer lugar, como actiidad principal, el equipo va a organizar el proyecto de evaluación mediante reuniones, planificaciones logísticas, calendario, acuerdo de puntos en común, etc. Se presentó un NDA para ser firmado por el equipo de evaluación y que así queden protegidos los secretos comerciales al respecto de la arquitectura en cuestión.

Hemos utilizado una planificación ágil para el desarrollo de la evaluación arquitectónica de forma que, llevando un control de versiones del documento mediante GitHub, hemos podido trabajar colaborativamente y ajustar las puestas en común del presente documento a lo largo de las reuniones propuestas.

En nuestro caso la evidencia de las reuniones realizadas se reflejan en el anexo 1. La primera es la puestá en común y presentación de la arquitectura, reflejada en el acta 1.

A continuación en presenta un calendario de reuniones propuestas.

Semana | Fase ATAM / Objetivos reunión | Reunión equipo evaluado 
-------|-------------------------------|------------------------
1/05 | Fase 0: preparación | N/A
6/05 | Fase 1: Presentación de ATAM | 9/05/2019, Acta 1
6/05 | Fase 1: Business drivers, presentación de la arquitectura | 10/05/2019, Acta 2
13/05 | Fase 1: Identificación de enfoques arquitectónicos, árbol de utilidad | N/A
13/05 | Fase 1: Generación del árbol de atributos de calidad | 13/05/19, Acta 3
13/05 | Fase 1: Enfoques arquitectónicos  | N/A
13/05 | Fase 2: Completa | N/A
20/05 | Fase 3: Follow-up y Conclusiones | N/A

:Planificación de reuniones

En el anexo 2 se recoge el NDA firmado entre las partes.

Una de las tareas que se ha realizado en esta fase es la identificación, dentro del equipo de evaluación, de los diferentes roles de equipo; en la tabla siguiente se recogen éstos.

Rol | Persona
----|--------
Líder del equipo | Luis Mata Aguilar
Líder de evaluación | Daniel Rodríguez Manzaneroo
Escriba de escenarios | Yeray Granada Layos
Escriba de actas | Carlos Gómez Robles
Entrevistador 1 | María Gallego Martín
Entrevistador 2 | Alejandro de la Fuente Perdiguero

:Roles del equipo ATAM

La planificación inicial pretende mantener realizando al equipo un trabajo constante condensado en iteraciones.  Mediante reuniones en el tiempo a lo largo de 4 semanas, se prevee que se podrá realizar en su totalidad la evaluación solicitada. Así mismo se preveen periodos de tiempo suficientemente condensados como para que existan huecos temporales en los que el equipo de evaluación pueda antender sus competencias externas a este proyecto.

# 3. Fase 1: Evaluación inicial

El proceso de evaluación principal definido en ATAM, se especifica en las fases 1 y 2, correspondientes a las secciones 3 y 4 de este documento.

En esa sección se reflejan los resultados de la primera fase en concreto. El equipo evaluador presenta al equipo del proyecto el proceso ATAM, se describen los pasos a seguir así como las preguntas a responder por el equipo evaluado.

A continuación se presentan Business Goals y Business Drivers del proyecto, incorporando las funciones principales del sistema.

## 3.1 Identificación de Business Goals y Business Drivers

Un Business Goal (objetivo de negocio) se define para un sistema como "la razón para construir dicho sistema" y un Business Driver como la manera en la que se pretende alcanzar dicho objetivo descrito en los Business Goals.

Los Business Goals definidos en el proyecto objeto de evaluación son los siguientes:
    
- 1. Lograr una gestión eficiente de las citas, de manera que el usuario sea capaz de pedir cita en hospitales y centros de salud de forma sencilla y veloz en cualquier momento.
    
- 2. Disposición de los usuarios de un método de asistencia automatizada. Cualquier usuario, especialmente aquellos con *un estado de salud delicado*, estén monitorizados. En caso de accidente, podrán recibir asistencia sanitaria lo más brevemente posible. 
    
- 3. Identificación de pacientes mediante escáner biométrico. Se presupone más rápido y eficiente el proceso de identificación, especialmente en accidentes y extingue la necesidad de que pacientes tengan que llevar documentación. Tipos considerados:
    * 3.1 Huella dactilar
    * 3.2 Iris

Los Business Drivers definidos en el proyecto objeto de evaluación son los siguientes:

- 1. Desarrollo de un sistema software de gestión de citas conectado con sistemas informáticos de la Seguridad Social y clínicas privadas participantes.
- 2. Desarrollo de aplicación móvil para el usuario final, podrán pedir tres tipos de cita:
    - 2.1 Cita normal: Cita al usuario en su centro médico habitual.
    - 2.2 Cita extraordinaria: Cita al usuario en centro diferente de su centro habtual (bien porque esté lejos físicamente) en cuyo caso se utilizarán servicios de geolocalización del dispositivo móvil. Se indicarán los centros médicos más cercanos y el usuario podrá elegir donde pedir cita.
    - 2.3 Cita de urgencia: Se le muestran al usuario hospitales cercanos que podrá elegir el más conveniente. El hospital recibirá una notificación informativa con la idea de evitar congestión en urgencias.

- 3. Monitorización a través de dispositivos IoT (Pulseras y relojes inteligentes). Mediante la aplicación móvil, los usuarios podrán vincular dispositivos IoT para detectar anomalías vitales como caída o paro cardíaco. En caso de detectar una anomalía semejante el sistema avisará a urgencias de forma automática para que el afectado reciba asistencia médica con la mayor brevedad posible.

- 4. Identificación de usuarios mediante escáner biométrico. Todo usuario dispone de un perfil virtual con sus datos personales (DNI, NIE, etc.), sus datos de Seguridad Social, seguro de salud privado si procede y datos biométricos bien sea huella dactilar o iris.

Hasta aquí la identificación de la documentación de partida. A continuación vamos a exponer nuestros criterios para una mayor conformidad en la evaluación. En cuanto a los Business Goals deben tenerse en cuenta los siguientes criterios:

- Tienen impacto *directo* en el sistema.
- Pueden implicar restricciones y otras limitaciones en el sistema.
- No están presentes en otros documentos.

Para conseguir estos objetivos es fundamental que su definición sea unívoca, siguiendo las recomendaciones de los profesores de la asignatura de Arquitectura y Diseño Software, plantearemos las características necesarias de la definición de Business Goals de acuerdo a la metodología SMART:

- S: *Specific* / Específico: que expresa claramente qué es exactamente lo que se quiere conseguir.
- M: *Measurable* / Medible: que se puedan establecer variables que determinen su éxito, fracaso o la evolución de los mismo a lo largo del tiempo.
- A: *Attainable* / Alcanzable: ha de tenerse en cuenta dimensiones de esfuerzo, tiempo y otros costes derivados para determinar si son viables, o si quedarán fuera del alcance.
- R: *Relevant* / Relevantes: útiles para el cliente.
- T: *Time-Related* / Con un tiempo determinado: ha de tener un contexto temporal.

**Business Goals: muy breves y genéricos, sin indicadores que permitan su evaluación. Les asignamos en lo que sigue los siguientes identificadores.**

Referencia | Business Goal | Comentario
-----------|---------------|-----------
BG1 | Lograr una gestión eficiente de las citas, de manera que el usuario sea capaz de pedir cita en hospitales y centros de salud de forma sencilla y veloz en cualquier momento. | Faltan indicadores que permitan verificar el Business Goal.
BG2 | Disposición de los usuarios de un método de asistencia automatizada. Cualquier usuario, especialmente aquellos con *un estado de salud delicado*, estén monitorizados. En caso de accidente, podrán recibir asistencia sanitaria lo más brevemente posible. | No hemos encontrado definición para estado de salud delicado en el documento original. Faltan indicadores.
BG3 | Identificación de pacientes mediante escáner biométrico. Se presupone más rápido y eficiente el proceso de identificación, especialmente en accidentes y extingue la necesidad de que pacientes tengan que llevar documentación. Tipos considerados: huella dactilar e iris. | Parece más un Business Driver de un Business Goal de integridad o eficiencia a la hora de identificar pacientes.

:Análisis de Business Goals

En la tabla siguiente se recoge el análisis de los Business Drivers, el cómo se pretenden conseguir los objetivos anteriormente descritos.

Referencia | Business Driver | Comentario
-----------|-----------------|-----------
BD1 | Desarrollo de un sistema software de gestión de citas conectado con sistemas informáticos de la Seguridad Social y clínicas privadas participantes. | No se menciona el servidor que posteriormente se usará para esta labor.
BD2 | Desarrollo de aplicación móvil para el usuario final, podrán pedir tres tipos de cita: normal, extraordinaria, urgencias. | Suponemos que este Driver está ligado al segundo Business Goal, por tanto, nos falta información sobre el cómo, no queda claro.
BD3 | Monitorización a través de dispositivos IoT (Pulseras y relojes inteligentes). Mediante la aplicación móvil, los usuarios podrán vincular dispositivos IoT para detectar anomalías vitales como caída o paro cardíaco. En caso de detectar una anomalía semejante el sistema avisará a urgencias de forma automática para que el afectado reciba asistencia médica con la mayor brevedad posible. | Más cercano a procedimiento que a Business Driver. Se entiende que se usarán dispositivos IoT. En nuestra consideración faltaría mencionar una aclaración al tipo de sistema crítico que se pretende construir, debido a la alta tasa de errores de estos dispositivos biométricos echamos en falta verificación de datos.
BD4 | Identificación de usuarios mediante escáner biométrico. Todo usuario dispone de un perfil virtual con sus datos personales (DNI, NIE, etc.), sus datos de Seguridad Social, seguro de salud privado si procede y datos biométricos bien sea huella dactilar o iris. | BG3 hecho Business Driver. El BG que pensamos para este Driver sería la identificación de usuarios mediante escáner biométrico.

:Análisis Business Drivers

## 3.2 Análisis de patrones arquitectónicos
Los patrones arquitectónicos ayudan a definir las características básicas y comportamientos de una aplicación. Conocer estas características, fortalezas y debilidades de cada patrón es necesario para poder elegir aquel que pueda suplir 

Uno de los aspectos más importantes de los patrones arquitectónicos es que están asociados a diferentes atributos de calidad. Esto quiere decir que existen algunos patrones que representan soluciones abstractas para problemas de rendimiento y otros pueden ser utilizados con éxito en sistemas que requieran de una alta disponibilidad. Al comienzo de la fase de diseño, un arquitecto de software escoge qué patrones arquitectónicos se adaptan más confortablemente a las necesidades de calidad deseadas para el sistema objetivo.

Entre los múltiples patrones arquitectónicos que existen, hemos visto en detalle como contenidos de la asignatura: 

- Layered Architecture
- Event-Driven Architecture
- Microkernel Architecture
- Microservices Architecture Pattern
- Space-Based Architecture

A continuación se prodece a la identificación de los patrones arquitectonicos usados.

### 3.2.1 Microservices

El equipo evaluado identifica en la vista de procesos un patrón arquitectónico de microservicios para los procesos realizados en el back-end del servidor donde se procesan los servicios. Sin embargo y debido a cariz de aplicación crítica que se presupone en los Business Goals, este patrón si bien puede crear aplicaciones implementadas que funcionen muy bien, en general este patrón no se presta a aplicaciones de alto rendimiento debido su naturaleza distribuida.

Por otro lado la testabilidad y la escalabilidad del sistema tratado se ven directamente afecadas positivamente por este patrón. De forma que cada proceso del sistema sería más sencillo de probar. Así mismo sería muy versátil para la adaptación de cambios o extensión de la aplicación para und desarrollo continuo en el futuro.

### 3.2.2 Event-Driven

El patrón principal que considera el equipo de evaluación que se ha seguido es el de *event-driven architecture* debido al uso de sistemas IoT con un servidor que gestiona las conexiones y una aplicación de móvil que gestione los eventos de análisis de mediciones de dichos dispositivos.

Se trata de que conforme se use la aplicación propuesta por el equipo original de diseño, los eventos se dispararán desde el primer momento. Primero en la captura de datos por los dispositivos y de ahí se propagarán eventos en forma de conexiones hasta los envíos de notificaciones a los centros médicos, tal y como se propone originalmente.

Además este tipo de patrón se usa en sistemas que requieran de una componente altamente asíncrona, como son los sensores IoT, lo cual minimizará el tiempo de respuesta, que además sería un atributo de calidad derivado de todos los Business Goals originalmente planteados.

Sin embargo este patrón arquitectónico no se ha visto considerado por el equipo de diseño.

## 3.3 Árbol de atributos de calidad

Un atributo de calidad es una propiedad medible o comprobable de un sistema que se utiliza para indicar cómo de bien el sistema satisface las necesidades de sus stakeholders.

En las tablas siguientes se recogen tanto atributos de calidad cómo el árbol de utilidad identificado por el equipo objeto de evaluación.


Atributo de calidad | Prioridad | Justificación
--------------------|-----------|--------------
Disponibilidad | Alta | En caso de emergencia el sistema necesita estar disponibl en cualquier día y hora del año.
Interoperabilidad | Alta | El sistema debe poder ser solicitado desde cualqueir dispositivo compatible.
Rendimiento | Alta | La respuesta del sistema debe resultar en el menor tiempo posible.
Seguridad (Security) | Media | Se tratan datos personales y sanitarios de pacientes. Según el RGPD son datos especialmente sensibles.
Escalabilidad | Media | El sistema debe tener la capacidad de soportar la interacción de un gran número de usuarios al mismo tiempo sin que se vea afectado su funcionamiento.
Portabilidad | Media | El sistema debe ser capaz de funcioanr correctamente en la mayoría de dispositivos.
Usabilidad | Baja | El sistema debe poder ser usado fácilmente.
Modificabilidad | Baja | El sistema debe poder ser modificable para facilitar el mantenimiento.
Testabilidad | Baja | El sistema se debe poder probar de forma sencilla.

:Atributos de calidad

Atributo de calidad | Atributo refinado | Architecture Significant Requirement
--------------------|-------------------|-------------------------------------
Disponibilidad | Tiempo disponible | El sistema estará disponible 24 del día, todos los días del año 
 - | Horario de actualización | En caso de que sea necesario mantenimiento o actualización, se llevará a cabo de 3 AM a 5 AM y no se inhabilitarán todas las funcionalidades, solo aquellas que vayan a ser actualizadas o mantenidas.
Interoperabilidad | Conexión con otros sistemas | El sistema se comunicará con los sistemas informáticos de la sanidad pública y las clínicas privadas que participen en el sistema
- | Conexión con dispositivos | El sistema será compatible con dispositivos de monitorización tipo relojes y pulseras inteligentes (inicialmente Apple Watch, Samsung Galaxy Watch, Samsung Gear Fit 2, Xiaomi Mi Band 2 y 3, Armazfit Bip, Fitbit Versa y Fitbit Inspire)
Rendimiento | Tiempo de respuesta (cita) | Cuando un usario solicita una cita el tiempo de respuesta del sistema para asignarle la cita no será mayor de 5 segundos.
- | Tiempo de respuesta (llamada a emergencias) | Cuando uno de los dispositivos de monitorización detecta una parada cardíaca o caída, el sistema responderá llamando a emergencias en un plazo máximo de 20 segundos.

:Árbol de utilidad original

A continuación, se procede al análisis de los atributos de calidad a partir de los Business Goals.

Atributo de calidad | Prioridad | Justificación   | Análisis realizado
--------------------|-----------|---------------|-------------------------------
Disponibilidad | Alta | Monitorización en tiempo real y detección de anomalías en tiempo real. Sistema de emergencia sanitario, por lo tanto crítico, y no puede fallar además de estar disponible en todo momento. | Se detecta de **GB1**. Consideramos que este sistema requiere de un nivel de disponibilidad muy alto, especialmente si hay vidas humanas de por medio. Por lo que categorizamos el sistema como crítico. Es un atributo de vital importancia.
Interoperabilidad | Alta | El sistema establecerá comunicaciones con sistemas informáticos ajenos como el de sanidad pública y será compatible con dispositivos de monitorización tipo relojes y pulseras inteligentes (IoT). | No se menciona en los BG, se presuone por la descripción y los drivers. Quizás asociable con **BG2**.
Rendimiento | Alta | Tiempo de respuesta, sincronización y reconocimiento de patrones biométricos en un tiempo aceptable. | Detectado de **BG1**. Sin métricas asociadas en BG.
Seguridad | Media | Solo podrán acceder a los datos personales las personas autorizadas. Los datos deben ser íntegros y protegidos frente a modificaciones. Sistema de autenticación. | En los BG no se recoge ninguna restricción de seguridad.
Usabilidad | Baja | Aplicación accesible y fácil de usar por ser de uso general con usuarios no expertos. | Nada deducible directamente de los BG. Es importante que sea usable si los usuarios finales de la aplicación no son expertos.
Modificabilidad | Baja | Se podrán realizar cambios en la aplicación con bajo coste. Pensamos que de forma continua sería una adición. No está contemplado en los Business Goals. | No deducible de los BG, quizás en **BG1** al tratar la gestión eficiente, lo cual implicaría que se pudiese modificar con facilidad, con la suficiente abstracción.
Testabilidad | Baja | Verificable y validable. El equipo quiere que sea fácil y rápida de probar. | Nada deducible delos BG. Pero al tratarse de un sistme crítico lo consideramos uno de los atributos más importantes. Debe estar todo probado y funcionar correctamente. No se puede tolerar que un fallo software se pueda cobrar una vida humana.
Escalabilidad | Media | Adaptable a cambios y extensiones. Márgenes planteados para aceptar aumentos significativos de datos y usuarios. | No deducible de los BG, importante para un sistema de este tipo, al ser un sistema ehealth que pretende captar usuarios de población civil en una ciudad.
Portabilidad | Media | Compatibilidad con Android e iOS | Nada derivable de los BG. No es muy importante que sea portable al principio debido a que las aplicaciones de un sistema de este tipo con el diseño adecuado, pueden ser fácilmente desplegadas a dispositivos finales.

:Ánalisis de atributos de calidad con Business Goals

A continuación, se analiza el árbol de utilidad, planteando cómo podrían quedar los atributos de calidad y refinados, la prioridad que identificamos en base al análisis de Business Goals, y el impacto global en la arquitectura y el valor de negocio, de cada uno de ellos. En algunos casos los atributos se verán modificados y en otros podría ser propuesta su eliminación. 

Atributo de calidad | Atributo refinado | Prioridad | Justificación de las decisiones
--------------------|-------------------|-----------|---------------------------
Confiabilidad | Disponibilidad | 1 | Al tratarse de un sistema crítico, debe estar planteado desde el primer momento en el diseño una disponibilidad 24/7 para evitar posibles daños a pacientes u otros inconvenientes. (**H,H**). ASR: Como cliente quiero que el sistema de alertas y emergencias esté disponible para detectarlas al menos un 99,90% del tiempo.
 - | Reconocimiento de patrones | - | La identificación de datos biométricos debe ser fehaciente a la realidad y ser confiable en cuanto a fallos, además de realizar la identificación en menos de medio segundo. (**H,L**). ASR: Como cliente quiero que el sistema reconozca con una tolerancia del 96% y en menos de medio segundo quién soy utilizando mis datos biométricos.
 Rendimiento | Time behaviour | 2 | Dada la cantidad de información que maneja el sistema y que ha de disponerse de ella en tiempo real, el tiempo de respuesta al usuario debe ser mínimo. (**H,H**). ASR: Como cliente quiero poder notificar emergencias en menos de 5 segundos y citas en menos de 20 segundos.
 - | Utilización de recursos | - | La sincronización de los dispositivos exige un escenario de tiempo real, por lo que deben minimizarse las diferencias de tiempo entre los datos en el servidor y los recién captados. (**H,H**). ASR: Como cliente quiero que la informaicón del sensor sea procesada por el sistema en menos de 2 segundos.
 Seguridad | Integridad | 3 | Los datos estarán protegidos frente a modificaciones no autorizadas (ej: Man-in-the-middle). (**M,H**). ASR: Como cliente quiero que mis datos personales estén protegidos y estén correspondidos con la realidad captada.
- | Control de accesos | - | Determinadas funciones del sistema deben estar restringidas a perfiles concretos de usuario. Como la calibración de dispositivos, o el acceso a identificadores biométricos. (**L,M**) ASR: Como cliente quiero que al sistema solo puedan acceder ciertos perfiles establecidos, especialmente a la configuración de dispositivos de captación de datos sensibles.
- | Confidencialidad | - | Dado el tipo de información personal y médica que procesa el sistema, ningunas terceras partes podrán acceder a estos datos personales. Los responsables de datos deben firmar y someterse a la responsabilidad del trato de dichos datos. (**H,H**). ASR: Como cliente quiero ejercer mi derecho de privacidad y proteger así mis datos personales.
Usabilidad | Facilidad de uso | 5 | Al tratarse de una aplicación de uso general y no especialista, debe ser fácil de usar para todo el mundo. (**L,M**). ASR: Como cliente quiero que la aplicación sea fácil de usar para garantizar un uso universal de la misma, especialmente al tratarse de un sistema e-health.
- | Accesibilidad | - | Además de ser fácil de usar, el sistema se contempla accesible universalmente, para establecer su uso a personas con limitaciones cognitivas, o sensoriales. (**M,L**). ASR: Como cliente quiero poder usar la aplicación sea cual sea mi condición física o psíquica.
Mantenibilidad | Escalabilidad | 4 | El sistema debe estar diseñado desde el principio para poder escalar horizontalmente, esto es, dar respuesta al incremento de usuarios previsto. (**H,M**). ASR: Como cliente quiero que el sistema sea escalable horizontalmente para no experimetar pérdidas de rendimiento con la popularización del uso en incrementos contemplados del 30% de usuarios, en un tiempo de 5 días/persona.
- | Modificabilidad | - | El sistema debe estar diseñado para soportar cambios de funcionalidad pertinentes de acuerdo con las posibles espeficicaciones de los stakeholders. Además se trata de un sistema en fases de prueba por lo que debe estar especialmente preparado para esto. (**M,H**). ASR: Como cliente el sistema debe poder ser lo suficientemente flexible como para incluir cambios de funcionalidad solicitados por stakeholders.
- | Testabilidad | - | Al tratarse de un sistema crítico, la correcta funcionalidad de todos los componentes debe estar verificada y validada con un umbral de tolerancia del 100% en los procesos críticos y un 80% en los componentes de interfaz. (**M,H**). ASR: Como cliente quiero que la aplicación esté validada y verificada, para no comprometer a los pacientes a fallos del sistema en cuestiones vitales.
Portabilidad | Adaptabilidad | 6 | La aplicación final de usuario del sistema debe poder ejecutarse tanto en Android como en iOS. Se pretende la universalización del sitema en cuanto a dispositivos. (**L,H**). ASR: Como cliente quero que el 100% de las funcionalidades de usuario se puedan realizar desde dispositivos Android e iOS.

:Árbol de utilidad propuesto

Del análisis de los atributos de calidad y árbol de utilidad, decidimos la reestructuración anterior por su compresión y en nuestra consideración, por su mejor etiquetado de atributos refinados. Así mismo eliminamos algunos atributos de calidad que consideramos que no tienen relevancia cruzada en el sistema. Siendo la nueva especificación propuesta más acorde a lo que se pretende conseguir con los Business Goals. Especialmente, cabe hacer incapié en los atributos refinados de **mantenibilidad**, que es el atributo de calidad nuevo que más sufre refactorización.

Así mismo, del análisis de los Business Goals, echamos en falta algún Business Goal conforme a como se presentó originalmente el sistema. Así mismo, no se presentaban con etiquetas reconocibles en el documento orginal por lo que hemos procedido a asignarles un nombre con el formato **BG1** para referirnos a ellos. A parte de ser muy breves, también consideramos que se han pasado por alto identificar métricas para los mismos.

## 3.4 Análisis de stakeholders

Grupos de prioridad identificados por el equipo de proyecto y nuestra reflexión al respecto.

## 3.5 Análisis de vistas

Para analizar el sistema usaremos el sistema de 4+1 vistas de Kruchten, que consiste en las siguientes vistas, las cuales detallaremos en esa subsección.

- Vista lógica
- Vista de procesos
- Vista de desarrollo
- Vista física o de despliegue
- Vista de escenarios

### 3.5.1 Vista lógica

#### Descripción

La vista lógica está relacionada con los requisitos funcionales y la estructra de clases conceptual que se va a usar en el sistema una vez construido. El objetivo es mostrar los componentes software del sistema y sus relaciones.

#### Análisis

Para la elaboración de esta vista han utilizado la notación UML de diagramas de clases estándar, donde comentan que cada entidad, representada por un cuadro con su nombre, donde mencionan la cardinalidad, pero no justfican el porqué de todas esas cardinalidades y creemos que es importante, puesto que para entender la vista en su totalidad, un apartado como las cardinalidades y la explicación de las mismas es necesario para comprender todas las relaciones. 

A nuestro parecer faltaría al menos una relación más, en concreto entre cliente y entidad sanitaria, donde la interacción entre ambos es directa, donde el cliente es atendido y donde la entidad sanitaria tiene registrado datos de cliente, y especialistas sanitarios que atienden a pacientes.

Se ha encontrado una inconsistencia en el Catálogo. En la vista hay un total de 5 entidades: Cliente, Pulsera, Móvil, Cuenta y Entidad Sanitaria. Sin embargo a la hora de mencionarlos y desarrollarlos en el catálogo, a lo que llamaban Cliente ahora se lo denomina Usuario. Deben tener el mismo nombre tanto en la vista como el catálogo.

Concluyendo, pese a la correcta justificación en su mayoría, la vista lógica debería tener algunas entidades y relaciones más.

#### Atributos de calidad

Respecto al Rationale se justifican la interoperablidad entre los distintos dispositivos, en este caso son móvil y pulsera asociados a una entidad sanitaria.


### 3.5.2 Vista de procesos

#### Descripción

El objetivo de un diagrama de procesos es mostrar uno o varios procesos del sistema software o del negocio mediante un flujo de trabajo. Este flujo comienza en un punto inicial y a continuación por una serie de tareas que pueden ser iterativas hasta llegar al punto final.

#### Análisis

Para el desarrollo del diagrama de actividades han utilizado el estándar UML, de forma que sea accesible y fácilmente interpretable para el mayor número de personas. 

Analizando la vista de procesos, la estructura basándonos en los “business goals” no me parece correcta por los siguientes motivos:

1.	Los avisos de emergencia no están bien definidos entre la pulsera, el teléfono móvil y el servidor que genera la llamada.
2.	No se hace mención a los sistemas biométricos para reconocer al paciente.


#### Justificación: Atributos de calidad

Se resalta la importancia de la interoperabilidad entre los diferentes elementos del sistema como son la pulsera, el teléfono móvil y el servidor para el correcto funcionamiento del sistema utilizando estos elementos para cumplir las funciones de la aplicación

### 3.5.3 Vista de desarollo

#### Descripción

El objetivo del diagrama de componentes es la organización del software en módulos para su desarrollo. Se pueden organizar los componentes en caoas o interfaces para su mejor comprensión. Lo cual lo facilitará la intuición de estos paquetes de software a la hora de implementar y desarrollar el sistema. 

#### Análisis

Se especifican tres diagramas en el documento original. Los tres corresponden a cada dispositivo del sistema: Entidad sanitaria, móvil y pulsera. Sin embargo no aparece por ningún lado el servidor ni los paquetes de componentes software de esta máquina. Lo consideramos una falta de información importante.

Se considera que todo el procese lo realiza esta máquina y pese a ello no disponemos de información en esta vista para su análisis. Sin embargo los paquetes software de los dispositivos finales están bien organizados. Los tres siguen arquitectura en capas.

Se desacopla correctamente la interfaz de la lógica y de la comunicación de cada dispositivo, permitiendo así un trabajo ágil y modificable como se indica en los atributos de calidad.


#### Justificación: Atributos de calidad

Con vistas a nuestro nuevo árbol de utilidad propuesto, cabría utilizar componentes de reflexión para saber el estado del sistema en cada momento y así, además de monitorizar datos de pacientes, podría monitorizarse el flujo de datos dentro del sistema y así poder redirigir los canales saturados. Esto llevaría el atributo de calidad de mantenibilidad a un nivel superior.

No se ve reflejada la disponibilidad que es el atributo más importante y debería ir de la parte del servidor, capaz de recoger los eventos lanzados por estos dispositivos.

Otra consideración a tener en cuenta es el uso de un patrón de broker, que podría aplicarse de cara a la captación de eventos por el servidor (ausente).

Si bien, se refleja la interoperabilidad en comunicación de los componentes, pero eliminamos este atributo de calidad por obvio, ya que se entiende que componentes diferentes de este sistema estarán conectados para interactuar tal y como se especifica.

Tampoco se refleja el atributo de rendimiento y seguridad por el lado de esta vista, para reflejarlo podrían incluirse paquetes de componentes que traten ambos problemas. 

### 3.5.4 Vista de despliegue

#### Descripción

La vista de despliegue tiene como objetivo asociar a cada elemento de las vistas anteriores un dispositivo físico donde se ejecutarán o residirán dichos componentes. Hablamos de redes, procesos, tareas, objetos, en diferentes nodos de este diagrama que podrán ser servidores, nodos de red, dispositivos finales ...

#### Análisis

En esta vista si aparece el componente de servidor como un nodo donde se ejecutan procesos. Esto no se veía reflejado en el diagrama de desarrollo. 

Aparece por primera vez una base de datos que no estaba contemplada en el documento hasta este momento. Se mencionan historiales de pacientes cosa no descrita en los BG.

Por lo demás queda lo suficientemente claro e ilustrativo de cómo se desplegará el sistema.

#### Justificación: Atributos de calidad

Según se indica, están bien mapeados los componentes del diagrama de procesos. Sin embargo no está bien mapeado con el diagrama de componentes, lo cual supone una inconsistencia.

Se refleja la interoperabilidad inicialmente planteada pero eliminada por el equipo de evaluación por motivos obvios.

Nos faltaría para tener un sistema consistente con sus BG, un servidor de backup para mantener la disponibilidad del sistema. Requisito de prioridad máxima, tal y como se ha identificado. Esto supondría una mejora de calidad importante para el sistema propuesto.

Para la disponibilidad en los canales de comunicación se proponen canales alternativos o cableados en caso de fallo para garantizar también la disponibilidad que este sistema crítico debe tener.

### 3.5.5 Vista de escenarios

#### Descripción

La vista de escenarios nos ofrece la posibilidad de mostrar las diferentes formas que tienen los usuarios de interactuar con el sistema.

#### Análisis 

En este caso para la vista de escenario se ha usado la notación UML estándar para casos de uso, explicando de forma muy completa cada elemento usado y su función. En concreto: Actor, caso de uso, ventana y asociación, cada uno representado con una imagen para su correcta identificación.

Se nos presenta un caso de uso que representa la interacción de los diferentes elementos del sistema. Consta de cuatro actores: Entidad sanitaria, Servidor, Móvil y Banda inteligente, y éstos, a su vez, estan asociados mediante relaciones con los elementos del sistema, que son: Gestión de citas, Recepción y gestión de datos biométricos y aviso de emergencia. En el caso de uso vemos como los distintos dispositivos y entidades interaccionan con los elementos del sistema, pero en ningún momento se muestra de que forma los usuarios/clientes hacen uso de ellos, por lo que sse podría añadir un quinto actor "Cliente". 

Respecto al catálogo, se justifica de forma correcta cada elemento del sistema.

#### Justificación: Atributos de calidad

Se comentan dos atributos de calidad:

- Interoperabilidad: en el caso de uso al tener elementos que se corresponden con dispositivos se puede observar fácilmente la relación que existe entre ellos y como interaccionan.

- Testabilidad: la explicación puede dar lugar a dudas, y además, no podemos ver si los elementos del sistema funcionan de forma correcta y/o óptima, por lo que se podría suprimir la testabilidad de este apartado al no tener una justificación del todo convincente. 

## 3.6 Identificación de puntos de sensibilidad

Se definen los puntos de sensibilidad de un sistema, como los componentes críticos para el éxito (correcto funcionamiento) del mismo. De la evaluación de la arquitectura propuesta hemos identificado los siguientes:

- PS1: Justificación
- PS2: Justificación ...

## 3.7 Identificación de puntos de equilibrio

Se definen los puntos de equilibrio de un sistema como una propiedad que afecta a más de un atributo de calidad o punto de sensibilidad. De la evaluación de la arquitectura propuesta, hemos identificado los siguientes:

- PE1: Justificación
- PE2: Justificación


## 3.8 Identificación de riesgos

Se define riesgo como una decisión arquitectónica que puede generar consecuencias indeseables a la luz de los requisitos de los atributos de calidad. De la evaluación de la arquitectura propuesta, hemos identificado los siguientes:

- R1: Descripción
- R2: Descripción

¿Posible métrica de coste de los riesgos?

# 4. Fase 2: Evaluación completa

En la segunda fase continúa el análisis de la arquitectura con los stakeholders del proyecto.

## 4.1 Análisis de escenarios existentes e identificaicón de nuevos escenarios

En está sección se presenta el análisis de escenarios. El objetivo es contar con suficiente información para poder tomar decisiones de diseño con conocimiento de causa y efecto, estableciendo un vínculo con los requisitos de los atributos de calidad que deben cumplirse.

### 4.1.1 Escenario 1

 Escenario: 1 | Como cliente quiero que el sistema ...
-------------|---------------------------------------
Atributo | Nombre de atributo
Contexto | -
Estímulo | -
Respuesta | -

:Escenario 1

Decisiones arquitectónicas | Decisión | Sensibilidad | Equilibrio | Riesgos | No riesgos 
---------------------------|----------|--------------|------------|------|----
 decision | - | - | - | - | -

:Escenario 1 decisiones

#### 4.1.1.1 Razonamiento

Explicación

#### 4.1.1.2 Diagrama arquitectónico


### 4.1.2 Escenario 2

 Escenario: 2 | Como cliente quiero que el sistema ...
-------------|---------------------------------------
Atributo | Nombre de atributo
Contexto | -
Estímulo | -
Respuesta | -

:Escenario 2

Decisiones arquitectónicas | Decisión | Sensibilidad | Equilibrio | Riesgos | No riesgos 
---------------------------|----------|--------------|------------|------|----
 decision | - | - | - | - | -

:Escenario 2 decisiones

#### 4.1.2.1 Razonamiento

Explicación

#### 4.1.2.2 Diagrama arquitectónico

### 4.1.3 Escenario 3

 Escenario: 3 | Como cliente quiero que el sistema ...
-------------|---------------------------------------
Atributo | Nombre de atributo
Contexto | -
Estímulo | -
Respuesta | -

:Escenario 3

Decisiones arquitectónicas | Decisión | Sensibilidad | Equilibrio | Riesgos | No riesgos 
---------------------------|----------|--------------|------------|------|----
 decision | - | - | - | - | -

:Escenario 3 decisiones

#### 4.1.3.1 Razonamiento

Explicación

#### 4.1.3.2 Diagrama arquitectónico

### 4.1.3 Escenario 4

 Escenario: 4 | Como cliente quiero que el sistema ...
-------------|---------------------------------------
Atributo | Nombre de atributo
Contexto | -
Estímulo | -
Respuesta | -

:Escenario 4

Decisiones arquitectónicas | Decisión | Sensibilidad | Equilibrio | Riesgos | No riesgos 
---------------------------|----------|--------------|------------|------|----
 decision | - | - | - | - | -

 :Escenario 4 decisiones

#### 4.1.4.1 Razonamiento

Explicación

#### 4.1.4.2 Diagrama arquitectónico

# 5. Fase 3:  Follow-up

La fase 3 se corresponde con el seguimiento, donde el equipo de evaluación produce y entrega un informe con los resultados finales de la evaluación. En primer lugar se distribuye a las partes interesadas fundamentales para asegurarse de que no contiene errores de comprensión, y una vez completada esta revisión se entrega a la persona encargada de la evaluación.

Al tratarse de un ejercicio académico las partes interesadas consideradas para la correcta compresión del documento serán bien profesores como cliente final y grupo evaluado como validadores de nuestro ejercicio.

# 6. Conclusiones de la evaluación

La presentación de conceptos así como la propia arquitectura propuesto por el equipo de proyecto para el Sistema --- resulta --- si bien consideramos que hay algunos aspectos mejorables en el planteamiento:

- Explicaciones
- 
- 
- 

# 7. Anexo 1: actas de reuniones

## 7.1 ACTA 1

### Fecha: 09/05/2019

### 7.1.1 Participantes

**Grupo responsable de la arquitectura**:
  
- Miguel Ángel Pérez Souza, bn0112
- Eric Romero Andrés, bn0111
- Alberto Sastre Gallardo, bn0195
- Alfonso Torres Sánchez, bn0107
- Carlos Vila Martín, bn0177
  
**Grupo ATAM**:
   
- Luis Mata Aguilar
- Carlos Gómez Robles
- Daniel Rodríguez Manzanero
- Yeray Granada Layos
- María Gallego Martín
- Alejandro de la Fuente Perdiguero
  
Roles ATAM | Miembro
-----------|---------
Team Leader | Luis Mata Aguilar
Evaluation Leader | Daniel Rodríguez Robles
Scenario scribe | Carlos Gómez Robless
Proceedings scribe | Yeray Granada Layoss
Questioner 1 | María Gallego Martín
Questioner 2 | Alejandro de la Fuente Perdiguero

:Roles ATAM acta 1

### 7.1.2 Introducción

### 7.1.3 Objetivos

### 7.1.4 Acuerdos

## 7.2 ACTA 2

### Fecha: 25/04/2019

### 7.2.1 Participantes

**Grupo responsable de la arquitectura**:
  
- Miguel Ángel Pérez Souza, bn0112
- Eric Romero Andrés, bn0111
- Alberto Sastre Gallardo, bn0195
- Alfonso Torres Sánchez, bn0107
- Carlos Vila Martín, bn0177
  
**Grupo ATAM**:
  
- Luis Mata Aguilar
- Carlos Gómez Robles
- Daniel Rodríguez Manzanero
- Yeray Granada Layos
- María Gallego Martín
- Alejandro de la Fuente Perdiguero
  
Roles ATAM | Miembro
-----------|---------
Team Leader | Alejandro de la Fuente Perdiguero
Evaluation Leader | Luis Mata Aguilar
Scenario scribe | Daniel Rodríguez Perdiguero
Proceedings scribe | Yeray Granada Layos
Questioner 1 | Carlos Gómez Robles
Questioner 2 | María Gallego Martín

:Roles ATAM acta 2

### 7.2.2 Introducción

### 7.2.3 Objetivos

### 7.2.4 Acuerdos

## 7.3 ACTA 3

### Fecha: 25/04/2019

### 7.3.1 Participantes

**Grupo responsable de la arquitectura**:
  
- Miguel Ángel Pérez Souza, bn0112
- Eric Romero Andrés, bn0111
- Alberto Sastre Gallardo, bn0195
- Alfonso Torres Sánchez, bn0107
- Carlos Vila Martín, bn0177
  
**Grupo ATAM**:
  
- Luis Mata Aguilar
- Carlos Gómez Robles
- Daniel Rodríguez Manzanero
- Yeray Granada Layos
- María Gallego Martín
- Alejandro de la Fuente Perdiguero
  
Roles ATAM | Miembro
-----------|---------
Team Leader | Daniel Rodríguez Manzanero
Evaluation Leader | Yeray Granada Layos
Scenario scribe | María Gallego Martín
Proceedings scribe | Alejandro de la Fuente Perdiguero
Questioner 1 | Luis Mata Aguilar
Questioner 2 | Carlos Gómez Robles

:Roles ATAM acta 3

### 7.3.2 Introducción

### 7.3.3 Objetivos

### 7.3.4 Acuerdos

# 8. Anexo 2: NDA

