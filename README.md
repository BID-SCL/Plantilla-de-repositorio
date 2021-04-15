
[![Analytics](https://gabeacon.irvinlim.com/UA-4677001-16/Plantilla-de-repositorio/readme?useReferer)](https://github.com/EL-BID/Plantilla-de-repositorio/)

## Plantilla de Documentación de Soporte y Uso de herramientas digitales - README.md

Esta es una plantilla basada en los estándares de la Guía de publicacion de herramientas digitales del BID. Sabemos que no existe un solo estándar para la documentación de soporte y uso de herramientas digitales pero hemos recopilado estas características importantes que debe tener un readme.md para facilitar el uso y amplificar el potencial de impacto de las mismas. Cualquier comentario o recomendación les pedimos generar un issue de consulta o escribirnos directamente a code@iadb.org.

Esta versión está adaptada para IADB-SCL con un enfoque en proyectos analíticos utilizando R, python o STATA principalmente.

## La plantilla empieza aquí 👇

<h1 align="center"> Nombre de la herramienta</h1>
<p align="center"> Logo e imagen o gif de la interfaz principal de la herramienta</p>
<p align="center"><img src="https://www.webdevelopersnotes.com/wp-content/uploads/create-a-simple-home-page.png"/></p> 

## Tabla de contenidos:
---

- [Badges o escudos](#badges-o-escudos)
- [Descripción y contexto](#descripción-y-contexto)
- [Guía de usuario](#guía-de-usuario)
- [Guía de instalación](#guía-de-instalación)
- [Estructura de repositorio](#estructura-de-repositorio)
- [Vulnerability Scanning](#vulnerability_scanning) 
- [Cómo contribuir](#cómo-contribuir)
- [Código de conducta](#código-de-conducta)
- [Autor/es](#autores)
- [Información adicional](#información-adicional)
- [Licencia](#licencia)
- [Limitación de responsabilidades - Solo BID](#limitación-de-responsabilidades)

## Badges o escudos
---
Es común en muchos repositorios open source el uso de badges o escudos para dar visbilidad el uso de microservicios, licencias, descargas, etc. Recomendamos revisar la iniciativa https://shields.io/ donde según consideres necesario podrás generar badges para tu repo. 

### Ejemplos de badges

- code coverage percentage: ![coverage](https://img.shields.io/badge/coverage-80%25-yellowgreen)
- stable release version: ![version](https://img.shields.io/badge/version-1.2.3-blue)
- package manager release: ![gem](https://img.shields.io/badge/gem-2.2.0-blue)
- status of third-party dependencies: ![dependencies](https://img.shields.io/badge/dependencies-out%20of%20date-orange)
- static code analysis grade: ![codacy](https://img.shields.io/badge/codacy-B-green)
- [SemVer](https://semver.org/) version observance: ![semver](https://img.shields.io/badge/semver-2.0.0-blue)
- amount of [Liberapay](https://liberapay.com/) donations per week: ![receives](https://img.shields.io/badge/receives-2.00%20USD%2Fweek-yellow)
- Python package downloads: ![downloads](https://img.shields.io/badge/downloads-13k%2Fmonth-brightgreen)
- Chrome Web Store extension rating: ![rating](https://img.shields.io/badge/rating-★★★★☆-brightgreen)
- [Uptime Robot](https://uptimerobot.com) percentage: ![uptime](https://img.shields.io/badge/uptime-100%25-brightgreen)

### Badges que solicitamos:
---
Solicitamos a los equipos que suman sus herramientas al catálogo de sumar el badge generado por el uso del microservicio de evaluación estática de código SonarCloud.

El badge se ve así y redirige al reporte de evaluación estática del último commit de la herramienta:

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=EL-BID_guia-de-publicacion&metric=alert_status)](https://sonarcloud.io/dashboard?id=EL-BID_guia-de-publicacion)


## Descripción y contexto
---
Esto es un archivo README. Debe contener la documentación de soporte uso de la herramienta digital. Las siguientes secciones son las secciones recomendadas que debes poner incluir en cualquier herramienta digital. Puedes descargar este archivo para que te sirva como plantilla.

Asegúrate de empezar este archivo con una breve descripción sobre las funcionalidades y contexto de la herramienta digital. Sé conciso y al grano.

## Guía de usuario
---
Explica los pasos básicos sobre cómo usar la herramienta digital. Es una buena sección para mostrar capturas de pantalla o gifs que ayuden a entender la herramienta digital.
 	

## Guía de instalación
---
Paso a paso de cómo instalar la herramienta digital. En esta sección es recomendable explicar la arquitectura de carpetas y módulos que componen el sistema.

Según el tipo de herramienta digital, el nivel de complejidad puede variar. En algunas ocasiones puede ser necesario instalar componentes que tienen dependencia con la herramienta digital. Si este es el caso, añade también la siguiente sección.

La guía de instalación debe contener de manera específica:
- Los requisitos del sistema operativo para la compilación (versiones específicas de librerías, software de gestión de paquetes y dependencias, SDKs y compiladores, etc.).
- Las dependencias propias del proyecto, tanto externas como internas (orden de compilación de sub-módulos, configuración de ubicación de librerías dinámicas, etc.).
- Pasos específicos para la compilación del código fuente y ejecución de tests unitarios en caso de que el proyecto disponga de ellos.

### Convenciones generales

#### Estructura de repositorio 
    .
    ├── docs                    # Documentation files (alternatively `doc`)
    ├── data                    # Data should not be uploaded to git!!.
    ├── src/project name        # Source files 
    ├── test                    # Automated tests (alternatively `spec` or `tests`)
    ├── tools                   # Tools and utilities
    ├── LICENSE
    ├── .gitignore              # [Template](https://github.com/BID-SCL/Plantilla-de-repositorio/blob/master/.gitignore)
    └── README.md


#### Guias de estilo 

Es mucho más fácil entender una gran base de código cuando todo el código contiene tiene un estilo coherente. 

* Python 
  * [General](https://www.python.org/dev/peps/pep-0008/) 
  * [SCL](https://github.com/BID-SCL/styleguides_scl/blob/master/code/python_styleguide.md) 

* R 
  * [General](https://google.github.io/styleguide/Rguide.html) 

* Stata: 
  * [General](https://journals.sagepub.com/doi/pdf/10.1177/1536867X0500500406) 
  * [SCL](https://github.com/BID-SCL/styleguides_scl/blob/master/code/stata_styleguide.md) 

* [C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
* [C# Style Guide](https://google.github.io/styleguide/csharp-style.html)
* [Swift Style Guide](https://google.github.io/swift/)
* [Objective-C Style Guide](https://google.github.io/styleguide/objcguide.html)
* [Java Style Guide](https://google.github.io/styleguide/javaguide.html)
* [Shell Style Guide](https://google.github.io/styleguide/shellguide.html)
* [HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)
* [JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)
* [AngularJS Style Guide](https://google.github.io/styleguide/angularjs-google-style.html)
* [Common Lisp Style Guide](https://google.github.io/styleguide/lispguide.xml)

## Vulnerability Scanning

- Todo proyecto debe pasar un test scann resolviendo bugs y vulnerabilidades de seguridad. Se puede utilizar el proyecto Opensource [SonarQube](https://github.com/SonarSource/sonarqube) para estos fines. 

#### Recomendaciones generales

- El uso de Dockerfiles es recomendado
- En caso de que el proyecto sea python incluir pip requirements.txt para especificar dependencias. 
- En caso de que el proyecto sea R incluir [packrat](https://github.com/rstudio/packrat)

### Dependencias
Descripción de los recursos externos que generan una dependencia para la reutilización de la herramienta digital (librerías, frameworks, acceso a bases de datos y licencias de cada recurso). Es una buena práctica describir las últimas versiones en las que ha sido probada la herramienta digital. 

    Puedes usar este estilo de letra diferenciar los comandos de instalación.


## Cómo contribuir
---
Esta sección explica a desarrolladores cuáles son las maneras habituales de enviar una solicitud de adhesión de nuevo código (“pull requests”), cómo declarar fallos en la herramienta y qué guías de estilo se deben usar al escribir más líneas de código. También puedes hacer un listado de puntos que se pueden mejorar de tu código para crear ideas de mejora. 


## Código de conducta 
---
El código de conducta establece las normas sociales, reglas y responsabilidades que los individuos y organizaciones deben seguir al interactuar de alguna manera con la herramienta digital o su comunidad. Es una buena práctica para crear un ambiente de respeto e inclusión en las contribuciones al proyecto. 

La plataforma Github premia y ayuda a los repositorios dispongan de este archivo. Al crear CODE_OF_CONDUCT.md puedes empezar desde una plantilla sugerida por ellos. Puedes leer más sobre cómo crear un archivo de Código de Conducta (aquí)[https://help.github.com/articles/adding-a-code-of-conduct-to-your-project/]

## Autor/es
---
Nombra a el/los autor/es original/es. Consulta con ellos antes de publicar un email o un nombre personal. Una manera muy común es dirigirlos a sus cuentas de redes sociales.

## Información adicional
---
Esta es la sección que permite agregar más información de contexto al proyecto como alguna web de relevancia, proyectos similares o que hayan usado la misma tecnología.

## Licencia 
---
[LICENCIA](https://github.com/BID-SCL/Plantilla-de-repositorio/blob/master/LICENSE.md)

La licencia especifica los permisos y las condiciones de uso que el desarrollador otorga a otros desarrolladores que usen y/o modifiquen la herramienta digital.

Incluye en esta sección una note con el tipo de licencia otorgado a esta herramienta digital. El texto de la licencia debe estar incluído en un archivo *LICENSE.md* o *LICENSE.txt* en la carpeta raíz.

Si desconoces qué tipos de licencias existen y cuál es la mejor para cada caso, te recomendamos visitar la página https://choosealicense.com/.

## Limitación de responsabilidades
Disclaimer: Esta sección es solo para herramientas financiadas por el BID.

El BID no será responsable, bajo circunstancia alguna, de daño ni indemnización, moral o patrimonial; directo o indirecto; accesorio o especial; o por vía de consecuencia, previsto o imprevisto, que pudiese surgir:

i. Bajo cualquier teoría de responsabilidad, ya sea por contrato, infracción de derechos de propiedad intelectual, negligencia o bajo cualquier otra teoría; y/o

ii. A raíz del uso de la Herramienta Digital, incluyendo, pero sin limitación de potenciales defectos en la Herramienta Digital, o la pérdida o inexactitud de los datos de cualquier tipo. Lo anterior incluye los gastos o daños asociados a fallas de comunicación y/o fallas de funcionamiento de computadoras, vinculados con la utilización de la Herramienta Digital.
