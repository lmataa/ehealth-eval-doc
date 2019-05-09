---
title: "Evaluación de una Arquitectura Software por medio de ATAM"
author: [ ]
date: "2019"
subtitle: "Segunda Práctica de Arquitectura de Software - UPM"
logo: capturas/logo.png
titlepage: "true"
toc: "true"
toc-own-page: "true"
listings-no-page-break: "true"
lof : "true"
lof-own-page: "true"
lot: "true"
lot-own-page: "true"
...

# 1. Introducción
> Posible cita aquí




## 1.1 Propósito del documento

Documento realizado por:

- Luis Mata Aguilar
- Carlos 
- Daniel 
- Yeray Granada 
- María Gallego Martín
- Alejandro
 
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

En esta fase de la evaluación ATAM, se le da comienzo al proceso de evaluación. En primer lugar, como actiidad principal, el equipo va a organizar el proyecto de evaluación mediante reuniones, planificaciones logísticas, calendario, acuerdo de puntos en común, etc. El equipo puede presentar un NDA para que sea firmado por el equipo de evaluación y que así queden protegidos los secretos comerciales al respecto de la arquitectura en cuestión.

Hemos utilizado...

Nuestro caso...

Se presenta un calendario de reuniones propuestas...

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
Líder de evaluación | Carlos
Escriba de escenarios | Daniel
Escriba de actas | Yeray
Entrevistador | María

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
BG1 | Lograr una gestión eficiente de las citas, de manera que el usuario sea capaz de pedir cita en hospitales y centros de salud de forma sencilla y veloz en cualquier momento. | -
BG2 | Disposición de los usuarios de un método de asistencia automatizada. Cualquier usuario, especialmente aquellos con *un estado de salud delicado*, estén monitorizados. En caso de accidente, podrán recibir asistencia sanitaria lo más brevemente posible. | -
BG3 | Identificación de pacientes mediante escáner biométrico. Se presupone más rápido y eficiente el proceso de identificación, especialmente en accidentes y extingue la necesidad de que pacientes tengan que llevar documentación. Tipos considerados: huella dactilar e iris. | -

:Análisis de Business Goals

En la tabla siguiente se recoge el análisis de los Business Drivers, el cómo se pretenden conseguir los objetivos anteriormente descritos.

Referencia | Business Driver | Comentario
-----------|-----------------|-----------
BD1 | Desarrollo de un sistema software de gestión de citas conectado con sistemas informáticos de la Seguridad Social y clínicas privadas participantes. | -
BD2 | Desarrollo de aplicación móvil para el usuario final, podrán pedir tres tipos de cita: normal, extraordinaria, urgencias. | -
BD3 | Monitorización a través de dispositivos IoT (Pulseras y relojes inteligentes). Mediante la aplicación móvil, los usuarios podrán vincular dispositivos IoT para detectar anomalías vitales como caída o paro cardíaco. En caso de detectar una anomalía semejante el sistema avisará a urgencias de forma automática para que el afectado reciba asistencia médica con la mayor brevedad posible. | -
BD4 | Identificación de usuarios mediante escáner biométrico. Todo usuario dispone de un perfil virtual con sus datos personales (DNI, NIE, etc.), sus datos de Seguridad Social, seguro de salud privado si procede y datos biométricos bien sea huella dactilar o iris. | -

:Análisis Business Drivers

## 3.2 Análisis de patrones arquitectónicos

Definición de patron arquitectonico seguida...

Particularidades y beneficios de los patrones arquitectonicos ...

Identificaicón de los patrones arquitectonicos usados...

## 3.3 Árbol de atributos de calidad

Un atributo de calidad es una propiedad medible o comprobable de un sistema...

Atributo de calidad | Prioridad | Justificación
--------------------|-----------|--------------
Atributo | Número | Texto

:Atributos de calidad

Atributo de calidad | Atributo refinado | ASR
--------------------|-------------------|----
Atributo | Refinado | ASR

:Árbol de utilidad original

A continuación, se procede al análisis de los atributos de calidad cruzados con los Business Goals.

Atributo de calidad | Prioridad | Justificación | Análisis
--------------------|-----------|---------------|---------
Atributo | Número | Texto del atributo | Nuestro análisis

:Ánalisis de atributos de calidad con Business Goals

A continuación, se analiza el árbol de utilidad, planteando cómo podrían quedar los atributos de calidad y refinados, la prioridad que identificamos en base al análisis de Business Goals, y el impacto global en la arquitectura y el valor de negocio, de cada uno de ellos. En algunos casos los atributos se verán modificados y en otros podría ser propuesta su eliminación. 

Atributo de calidad | Atributo refinado | Prioridad | Justificación
--------------------|-------------------|-----------|--------------
Atributo (nuevo o no) | Atributo refinado (nuevo o no) | Prioridad nuestra | Justificación de las decisiones tomadas

:Árbol de utilidad propuesto

Del análisis de los atributos de calidad y árbol de utilidad, detectamos que, ...

Así mismo, del análisis de los Business Goals ...

## 3.4 Análisis de stakeholders

Grupos de prioridad identificados por el equipo de proyecto y nuestra reflexión al respecto.

## 3.5 Análisis de vistas

Intro de sección

- Vista lógica
- Vista de procesos
- Vista de desarrollo
- Vista física o de despliegue
- Escenarios

### 3.5.1 Vista lógica

### 3.5.2 Vista de procesos

### 3.5.3 Vista de desarollo

### 3.5.4 Vista de despliegue

### 3.5.5 Vista de escenarios

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

### Fecha: 25/04/2019

### 7.1.1 Participantes

Grupo responsable de la arquitectura:
  
- 
- 
- 
- 
- 
  
Grupo ATAM:
  
- 
- 
- 
- 
- 

Roles ATAM | Miembro
-----------|---------
Team Leader | -
Evaluation Leader | -
Scenario scribe | -
Proceedings scribe | -
Questioner | - 

:Roles ATAM acta 1

### 7.1.2 Introducción

### 7.1.3 Objetivos

### 7.1.4 Acuerdos

## 7.2 ACTA 2

### Fecha: 25/04/2019

### 7.2.1 Participantes

Grupo responsable de la arquitectura:
  
- 
- 
- 
- 
- 
  
Grupo ATAM:
  
- 
- 
- 
- 
- 

Roles ATAM | Miembro
-----------|---------
Team Leader | -
Evaluation Leader | -
Scenario scribe | -
Proceedings scribe | -
Questioner | - 

:Roles ATAM acta 2

### 7.2.2 Introducción

### 7.2.3 Objetivos

### 7.2.4 Acuerdos

## 7.3 ACTA 3

### Fecha: 25/04/2019

### 7.3.1 Participantes

Grupo responsable de la arquitectura:
  
- 
- 
- 
- 
- 
  
Grupo ATAM:
  
- 
- 
- 
- 
- 

Roles ATAM | Miembro
-----------|---------
Team Leader | -
Evaluation Leader | -
Scenario scribe | -
Proceedings scribe | -
Questioner | - 

:Roles ATAM acta 3

### 7.3.2 Introducción

### 7.3.3 Objetivos

### 7.3.4 Acuerdos

# 8. Anexo 2: NDA

