---
title: Proyecto Genkidama
root: "/docs"
parents: ["Material Complementario"]
---

#Introducción
Tanto para la asignatura de desarrollo web, como Arquitectura de software, se considerará un proyecto para cada equipo, en el que podrán desarrollar un sitio web destinado a la gestión documental a través de múltiples herramientas que permitirán a los alumnos llevar a cabo un sitio con todos los beneficios de la nube y las últimas tecnologías de desarrollo. 

##Beneficios del proyecto
El valor de las empresas modernas, son sus bases de conocimientos, esto les permite gestionar la documentación que utilizan los miembros de su equipo y sus clientes. El uso de documentos portables, como [Markdown](https://es.wikipedia.org/wiki/Markdown) permite ambientes colaborativos de gestión documental con el fin de que las empresas sean dueñas del conocimiento generado por sus equipos.

##Descripción General

Para el caso del presente proyecto, los alumnos generarán documentación de lo aprendido. Como parte de la gestión documental, tendrán documentación a nivel de proyecto (Wiki de Azure Devops) y determinarán la mejor documentación hacia el sitio web. Cada alumno deberá generar al menos un documento para cada asignatura con lo que aprendieron en el proyecto, el cual será definido en el transcurso de cada una de las asignaturas.

Además deberán considerar funcionalidades a elección de cada equipo, que conecten a un servidor en la nube, utilizando la que sea de su preferencia y las tecnologías propuestas más adelante.

#Tecnologías utilizadas


##Arquitectura del lado del cliente
Para el proyecto se darán las bases iniciales para crear rápidamente un sitio web de gestión documental, a partir de dicho sitio los equipos podrán poner en práctica los contenidos de ambas asignaturas.

Las tecnologías necesarias para el proyecto son las siguientes:

###GatsbyJs
GatsbyJs es un generador de sitios estáticos que permite obtener rápidamente un sitio web  con todas las necesidades actuales, esto permitirá crear sitios con las siguientes características. 

1. Performance sobre cualquier otra tecnología.
2. SEO Friendly, los sitios generados bajo esta tecnología permiten tener un 100% de compatibilidad SEO.
3. PWA (Aplicaciones Web Progresivas), los sitios de gatsby permiten rápidamente generar aplicaciones web y aplicaciones móviles.
4. GraphQl integrado.
5. Compatibilidad ReactJs.
6. Gestión nativa de documentos Markdown.

El principal motivo para el uso de esta tecnología, tiene relación con la rapidez en la que los alumnos podrán poner en práctica el uso de ReactJs, para crear sitios web en base a componentes.


###Javascript/Typescript
Para el proyecto será requisito dominar JavaScript como lenguaje del lado del cliente (o del lado del servidor, como se verá más adelante). Se alentará el uso de TypeScript, un lenguaje tipado que es usado como una pila superior a JavaScript, que permite tener mayor control del código.


###GraphQL
Gatsby incluye una pequeña base de datos de solo lectura que es usada con GraphQL, esto permitirá rápidamente a los alumnos reconocer el lenguaje de consultas utilizado por esta cada vez más utilizada tecnología, sin mediar la creación del modelo. A través de esta última podrán mejorar la calidad del sitio y agregar más funcionalidades.

###Gestión del proyecto
Para la gestión del proyecto se usará Azure Devops, lo que permitirá mantener seguimiento de cada una de las actividades y como derivan en el producto final. Para la gestión de las tareas se hará uso de Kanban, permitiendo un flujo simple de gestión.

###Control de calidad
En el transcurso del proyecto se solicitará al menos un test unitario que permita establecer la calidad del código a presentar. 

###CI-CD
Integración continua y Entrega continua permite automatizar los procesos relacionados con integración (asegurando el versionado correcto, en relación a los anteriores) y entrega (liberación automatizada en la nube o local). 

Para el proyecto inicial se mostrará un ejemplo simple con [netlify](https://www.netlify.com/) que permitirá mantener actualizado un sitio público, cada vez que se realice un [pull request](https://www.atlassian.com/git/tutorials/making-a-pull-request).

En el proyecto deberán usar este como base de conocimiento, para generar la propia de acuerdo a las opciones que se presentarán como contenido del proyecto.

###Autenticación
Para el proyecto se usará un servicio de autenticación que permitirá el acceso privado a algunos contenidos, para este propósito podrá usar la nube u otro servicio de autenticación, como Auth0.

###Artefactos 
Uno de los componentes construidos con React deberá ser subido a la nube como un micro programa empaquetado a través de un repositorio gratuito en Azure Devops u otro repositorio, esto permitirá abordar la gestión de componentes.

###Control de versiones
Como parte fundamental del proyecto, la gestión de versionado de archivos, colaboración y su distribución conformarán parte esencial de todo el proceso.

##Arquitectura del lado del servidor
El proyecto contempla operaciones lógicas que serán gestionadas en la nube, con el lenguaje que cada alumno determine y la nube que cada equipo defina.

Para el trabajo se deberá considerar alguna funcionalidad del lado del servidor que permita conectar con la aplicación del lado del cliente. 

Estas funcionalidades pueden ser determinadas por el equipo, algunas de estas pueden ser:

1. Comentarios asociados a los artículos.
2. Formulario de contacto.
3. Reserva de algún evento ficticio.
4. etc.

Con el fin de materializar la funcionalidad del lado del servidor, durante el proyecto se verán las siguientes tecnologías.

##FAAS (Functions as a Service) 
Functions as a Service es parte de la [arquitectura serverless](https://martinfowler.com/articles/serverless.html), y es la tecnología utilizada por los principales proveedores en la nube ([AWS](https://aws.amazon.com), [Azure](https://azure.microsoft.com) y [Google Cloud Platform](https://cloud.google.com/)), también existen imágenes de [Dockers](https://www.openfaas.com/) que implementan esta tecnología.

Como parte del contenido veremos los fundamentos y las directrices para el uso de esta en AWS y Azure.

Los alumnos deberán elegir una de las tecnologías presentadas, y utilizar el lenguaje de su preferencia.


##Bases de datos
En el contenido del curso veremos las diferencias de las bases de datos en la nube, costos relacionados y los beneficios de las bases de datos administradas. 

Como parte del trabajo de cada equipo, deberán elegir una de las bases de datos mostradas y usarla como parte del proyecto.


##Test Unitarios
Cada uno de los alumnos deberá crear al menos un test unitario que valide su propio código, podrá ser del lado del cliente o del lado del servidor.









  










