## Capítulo V: Product Implementation, Validation & Deployment
### 5.1. Software Configuration Management.
#### 5.1.1. Software Development Environment Configuration.
En esta sección especificaremos y detallaremos las plataformas y software que usamos como equipo para la realización de nuestro startup.

- GitHub: En esta plataforma es donde crearemos nuestro repositorio donde realizaremos los avances de nuestro startup. Además, nos ayuda a tener un mejor control en el trabajo de equipo debido a que se puede visualizar el avance de cada integrante a través de los commits.
https://github.com<br></br>

- Whatsapp: Es una aplicación de mensajería instantánea multiplataforma que permite a los usuarios enviar mensajes de texto, voz y multimedia, así como realizar llamadas y videollamadas gratuitas a través de una conexión a Internet. Con una interfaz intuitiva y amplia disponibilidad en dispositivos móviles y de escritorio, WhatsApp se ha convertido en una herramienta omnipresente para la comunicación personal y empresarial en todo el mundo.
https://whatsapp.com/<br></br>

- Visual Studio Code: Es un editor de código fuente ligero pero potente, desarrollado por Microsoft, que ofrece una amplia gama de características para programadores. Con soporte para múltiples lenguajes de programación, extensiones personalizables, integración con control de versiones y depuración, así como una interfaz intuitiva y altamente personalizable, Visual Studio Code se ha convertido en una opción popular para desarrolladores de software en todo el mundo.
https://code.visualstudio.com/<br></br>

- Git: Sistema de control de versiones más usado, es un requisito para poder realizar los commits en Github.
https://git-scm.com/downloads<br></br>

#### 5.1.2. Source Code Management.
##### Gestión del Código Fuente: 

En esta sección, explicaremos cómo gestionamos y seguimos el desarrollo del código en Ruedarent. Utilizamos GitHub como plataforma y Git como sistema de control de versiones.

- Repositorio en GitHub para el Landing Page: https://github.com/upc-pre-202401-si720-si91-Ruedarent/Ruedarent-Landing-Page

Se ha implementado el flujo de trabajo GitFlow para una gestión efectiva de los cambios en el código de la aplicación y la administración de las ramas en cada repositorio. Este flujo de trabajo implica la creación de dos ramas principales:

- **main:** También conocida como "master", esta rama alberga la versión más estable y lista del proyecto que está lista para ser lanzada a producción.
- **develop:** Esta rama es donde se integra el contenido de las nuevas características (features). Se desarrolla de forma paralela a la rama main.

Además de estas ramas principales, se utilizan ramas auxiliares para diferentes propósitos:

- **feature:** Estas son ramas donde se desarrollan las funcionalidades del proyecto de forma independiente. Una vez completadas, se fusionan con la rama develop.
- **release:** Estas ramas se utilizan para preparar la próxima versión del programa. Aquí se realizan las pruebas finales y se corrigen errores menores antes del lanzamiento oficial. Una vez completado este proceso, los cambios se fusionan primero con la rama develop y luego con la rama main.
- **hotfix:** Estas ramas se utilizan para corregir errores críticos que surgen en producción y requieren una solución urgente. Se derivan de la rama main y se fusionan tanto con esta como con la rama develop.

El formato de nomenclatura utilizado para las ramas sigue una convención específica, donde las ramas feature tienen el formato "feature/feature-name" y las ramas release siguen el formato "release/x.y.z", siguiendo las pautas de Semantic Versioning 2.0.0. En este formato, X, Y y Z son números enteros positivos que indican la versión mayor, menor y de parche, respectivamente. Cada incremento en estas versiones sigue reglas específicas para garantizar la compatibilidad y la comprensión de los cambios realizados.

##### - Commits Conventions:
En Ruedarent, seguimos la convención de commits convencionales para nuestros mensajes de confirmación. Estos mensajes siguen una estructura específica: 

- `<tipo>[ámbito opcional]: <descripción>` con opciones para el cuerpo y el pie del mensaje.
- Tipo "fix": Utilizamos este tipo de commit cuando se soluciona un error que afecta a los usuarios.
- Tipo "feat": Utilizamos este tipo de commit cuando se agrega una nueva característica para los usuarios.
- "BREAKING CHANGE": Utilizamos esta etiqueta en el pie del mensaje para comunicar cambios significativos en la API.

También se permiten otros tipos de commits, como "perf" (rendimiento), "build" (cambios en la compilación), "docs" (cambios en la documentación), "refactor" (refactorización), "style" (cambios de
formato), "test" (agregar o refactorizar pruebas), entre otros.

Estas prácticas nos ayudan a mantener un control efectivo del desarrollo de Ruedarent y a comunicar claramente los cambios en nuestro código fuente.

#### 5.1.3. Source Code Style Guide & Conventions.
En Ruedarent se han adoptado varias convenciones de estilo para el desarrollo de código en diferentes lenguajes y tecnologías:

##### HTML y CSS (Google HTML/CSS Style Guide)
- Se declara el tipo de documento al principio del archivo con `<!DOCTYPE html>`.
- Se incluyen los meta tags pertinentes.
- El elemento `<title>` se coloca dentro de las etiquetas `<head>`.
- Se utiliza una indentación de dos espacios.
- Se emplean minúsculas para los elementos HTML, atributos, propiedades, valores y selectores CSS.
- Los atributos de los elementos HTML se encierran entre comillas.
- Cada elemento HTML debe tener su etiqueta de cierre.
- Se evitan líneas de código excesivamente largas.
- Se especifica el ancho y alto de las imágenes, junto con un texto alternativo (alt).

##### JavaScript (Google Java Style Guide)
- Cada línea de código debe terminar con un punto y coma (`;`).
- Tanto las variables como las funciones deben seguir la convención CamelCase.
- Los valores de strings se encierran entre comillas simples.
- La indentación del contenido es de +2 espacios.
- Se prefiere el uso de `let` y `const` en lugar de `var` para definir variables.

##### Gherkin (Gherkin Conventions for Readable Specifications)
- Se emplean las palabras "Given", "When", "Then" y "And" para describir los pasos del escenario.
- Los pasos que comienzan con "And" se indentan.
- Se añaden líneas en blanco entre pasos.
- Los parámetros se encierran entre comillas simples.
- Se utiliza un comentario separador y dos líneas en blanco entre cada escenario.

##### C# (Microsoft C# Coding Conventions):
- Los nombres de los paquetes se escriben en minúsculas, las clases en UpperCamelCase y los métodos en lowerCamelCase.
- La indentación se realiza con 2 o 4 espacios, sin utilizar tabulaciones.
- Se dividen las líneas de código que excedan los 100 caracteres.
- Los archivos C# deben tener el mismo nombre que la clase que contienen, y esta debe ser única y pública.
- Después de cada declaración, se agrega un salto de línea.

Estas convenciones ayudan a mantener un código limpio, legible y consistente a lo largo de todo el proyecto.

- US01:

![image.png](https://i.ibb.co/rx4Ls53/image.png)

- US02:

![image.png](https://i.ibb.co/5FvNxDR/image.png)

- US03:

![image.png](https://i.ibb.co/sPGSf36/image.png)

- US04:

![image.png](https://i.ibb.co/b2CgqQS/image.png)

- US05:

![image.png](https://i.ibb.co/SsxVHm4/image.png)

#### 5.1.4. Software Deployment Configuration.

En esta sección, abordaremos el despliegue de nuestra Landing Page mediante el servicio automatizado en la nube de GitHub Pages. A continuación, se describirán los pasos para lograr este objetivo.

- Es crucial asegurarnos de que el repositorio esté configurado correctamente, ya que posteriormente lo desplegaremos con GitHub Pages:

![image.png](https://i.ibb.co/3WgXRTv/Desplegar-Git.png)

- Accedemos al GitHub Pages:

![image.png](https://i.ibb.co/P12sv1T/Git-Hub-Page.png)

- Después de haber establecido nuestro repositorio, procedemos a asignar las diversas "User Stories" entre los miembros del equipo para llevar a cabo el desarrollo de nuestra Landing Page. Además, creamos ramas individuales según sea necesario. Esto permitió que cada miembro trabajara de manera eficiente sin conflictos.

![image.png](https://i.ibb.co/bzXgWHb/image.png)

- Una vez que hayamos guardado la configuración, GitHub Pages iniciará el proceso de despliegue de nuestra Landing Page. Aquí podremos seguir el proceso de despliegue y, una vez que se complete con éxito, se generará un enlace que nos permitirá acceder a nuestra Landing Page.

![landingpage.png](https://i.ibb.co/qdvJgTR/image.png)

### 5.2. Landing Page, Services & Applications Implementation.
#### 5.2.1. Sprint 1.
#### 5.2.1.1. Sprint Planning 1.

En este sección, están las reuniones que se realizaron para llevar a cabo la Landing Page.

| Sprint # | Sprint #1 |
| -------- | --------|
| Sprint Planning Background |
| Date | 2024-04-10 |
| Time | 05:25 PM |
| Location | Google Meet (virtual) |
| Prepared by | Gallo Quintana, David Ivanoff |
| Attendes (to planning meeting) | Gallo Quintana, David Ivanoff / La Rosa, Alejandro / Calisaya Sánchez, Juan Jesús  / Oneglio, Beth / Huarcaya Niurka |
| Sprint Goal & User Stories |    |
| Sprint 1 Goal | Realizar la Landing Page |
| Sprint 1 Velocity | 45|
| Sum of Story Points | 40 |

#### 5.2.1.2. Sprint Backlog 1.

| id   | Title                  | Id  | Title                                                    | Description                                                                                                   | Estimations(Hours) | Assigned To   | Status(To-do /InProcess/ToReview/Done) |
| ---- | ---------------------- | --- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------ | ------------- | -------------------------------------- |
| HU01 | Barra de navegación de la landing page     | TS01 |Header and NavBar responsivos (Desarrollado en HTML, CSS y JS).          | Implementación del header y la barra de navegación, siguiendo los estándares “Responsive”  | 8                  | David | Done                                   |
| HU02 | Sección de beneficios    | TS02 | Sección de Beneficios (Desarrollado en HTML, CSS y JS).       | Implementación de la sección de Beneficios en la Landing Page, siguiendo los estándares “Responsive”  | 8                 | Alejandro | Done                                   |
| HU03 | Sección de nosotros           | TS03 | Sección de nosotros (Desarrollado en HTML, CSS y JS).                              | Implementación de la sección nosotros en la Landing Page, siguiendo los estándares “Responsive”.           | 8                  | Beth   | Done                                   |
| H04 | Visualización de las redes sociales/Footer del Landing Page | TS04 | Seccion de footer (Desarrollado en hTML, CSS y JS). | Implementación de visualización de redes | 8 | Niurka | Done
|H05 | Seccion de contactos en la Landing Page | TS05 | Sección footer (Desarrollado en HTML , CSS y JS) | Implementación de footer | 8 | Juan |Done

#### 5.2.1.3. Development Evidence for Sprint Review.

| Repository | Branch | Commit Id | Commit <br>Message | Commit <br>Message Body | Commited <br>on (Date) |
|:-------------:|:---------------:|:-------------:|:-------------:|:---------------:|:-------------:|
| [Ruedarent <br>Landing Page](https://github.com/upc-pre-202401-si720-si91-Ruedarent/Ruedarent-Landing-Page) | main | 878eb379530bba34ba873c65bd1910058b1a443e | Initial commit |  | 30/03/2024 |
|  | feat/section-vehicles | 04043ab2c41e879a1395a62d32e81746de41bb5e | feat: added/section-vehicles |  | 12/04/2024 |
|  | feat/section-vehicles | 87ae681f43e7832d266ccaf06d5b59ce40495ea4 | feat: added Section vehicles |  | 12/04/2024 |
|  | feat/section-benefits | 33c1fdd6a89424db5ef9e429383daf02934dc0d8 | feat: added section benefits |  | 12/04/2024 |
|  | feat/section-alertas | 8e00870b2827fa0be585af6e162d2bf5c2d3d568 | Add: Alert section |  | 13/04/2024 |
|  | feat/section-us | e6d0b79d5946afc4a1c93e31e76dcf0843435738 | feat: added us index.html |  | 13/04/2024 |
|  | feat/section-us  | 0b339e0a7775226891d44434ae18e753b4e910a4 | feat: added us style.css |  | 13/04/2024 |
|  | feat/section-alertas | 42929bb5d7ba742ed1fa44a54e9e4953c3f0f291 | Merge branch 'feat/section-benefits' into feat/section-alertas |  | 14/04/2024 |
|  | releases | 833e5f8391bedb6dea5e81c17ba3736486e57e4e | feat: merged sections |  | 14/04/2024 |

#### 5.2.1.4. Testing Suite Evidence for Sprint Review.

Durante este sprint, hemos llevado a cabo las pruebas de aceptación utilizando la herramienta Gherkin. Puedes encontrar los escenarios de estas pruebas dando click aqui: [https://github.com/upc-pre-202401-si720-si91-Ruedarent/Ruedarent-Acceptance-Tests](https://github.com/upc-pre-202401-si720-si91-Ruedarent/Ruedarent-Acceptance-Tests).

| Repository | Branch | Commit Id | Commit <br>Message | Commit <br>Message Body | Commited <br>on (Date) |
|:-------------:|:---------------:|:-------------:|:-------------:|:---------------:|:-------------:|
| [Ruedarent <br> Acceptance Tests](https://github.com/upc-pre-202401-si720-si91-Ruedarent/Ruedarent-Acceptance-Tests) | main | f188729754140b486ecc985eacccb62a60b52b2b | Initial commit |  | 14/04/2024 |
|  | main | d2382ffd3319c3b7f5bcf2292d1a743f489f918d | feat: added acceptance tests epic01 |  | 15/04/2024 |

#### 5.2.1.5. Execution Evidence for Sprint Review.

En esta entrega, el equipo Ruedarent ha logrado completar con éxito la creación de la Landing Page. Esta proporcionará detalles precisos sobre nuestra misión como startup, además de ofrecer información sobre los servicios que proporcionamos en nuestra aplicación web.

Enlace del deploy del Landing Page de Ruedarent en GitHub Pages: https://upc-pre-202401-si720-si91-ruedarent.github.io/Ruedarent-Landing-Page/

Sección de header donde se encuentra el menu de navegación principal y el Banner donde  se muestra un mensaje con una imagen acerca de Ruedarent:

![Execution Evidence](https://i.ibb.co/5kMr3qt/page1.png)

Sección de inscribirse para que los usuarios den su apoyo e información básica:

![inscribase](https://i.ibb.co/ym2RzSk/inscribase.png)

Sección de vehículos para visualizar que tipo ofrecemos: 

![vehículos](https://i.ibb.co/XtdW49h/vehiculos.png)

Sección de beneficios para  mostrar a los usuarios lo que se obtiene al elegir a Nosotros:

![beneficios](https://i.ibb.co/JnWZDB1/beneficios.png)

Sección de nosotros, donde se muestra información relevante sobre la startup y sus valores:

![nosotros](https://i.ibb.co/gM9J3j3/nosotros.png)

Sección de contacto y footer con enlaces a redes sociales y un formulario de contacto:

![contacto y footer](https://i.ibb.co/fqGymMs/contactoyfooter.png)

Link del video explicativo del Landing Page de Ruedarent: [https://upcedupe-my.sharepoint.com/personal/u202121935_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu202121935%5Fupc%5Fedu%5Fpe%2FDocuments%2FDetalle%20del%20landing%20page%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview](https://upcedupe-my.sharepoint.com/personal/u202121935_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu202121935%5Fupc%5Fedu%5Fpe%2FDocuments%2FDetalle%20del%20landing%20page%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview)

#### 5.2.1.6. Services Documentation Evidence for Sprint Review.

En esta entrega, nos enfocamos en Landing page, por lo que no fue necesario ningún servicio adicional.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review.

En este caso se uso GitHub Pages, para desplegar la Landing page, el cual nos sirvio para, a partir de un código en un repositorio poder desplegar la página. Enlace de la landing page: [https://upc-pre-202401-si720-si91-ruedarent.github.io/Ruedarent-Landing-Page/](https://upc-pre-202401-si720-si91-ruedarent.github.io/Ruedarent-Landing-Page/)

#### 5.2.1.8. Team Collaboration Insights during Sprint.

Para llevar a cabo este proyecto se usaron distintas herramientas como Visual Studio Code, Webstorm; junto con manejo de versiones en Git. En este caso se dividio la landing page mostrada anteriormente en sectores, a partir de esto cada uno presentó su parte y luego un miembro juntó las partes para finalmente tener el resultado deseado.

![Commit1](https://i.ibb.co/QbLdLqC/commits1.png)

## Conclusiones

- Para tener éxito durante la elaboración del proyecto es necesario que todos los integrantes participen y colaboren de manera equitativa, para que el proyecto pueda ser finalizado de manera rápida.

- Es bastante importante la realización de User stories junto con product backlog para definir las necesidades de los usuarios asi como clasificarlos por su importancia, esto con el objetivo de realizar las necesidades más importantes primero.

- Para tener éxito, es esencial abordar el riesgo de errores funcionales mediante pruebas y mejoras continuas.

## Bibliografía

- Gutiérrez Flores, R. R., & Márquez Cabezas, J. L. (2020).       
Análisis de los factores asociados al crecimiento del tráfico vehicular, mediante un método dinámico intertemporal en Lima Metropolitana, periodo 1990-2018. [Tesis de bachiller, Universidad San Ignacio de Loyola]. https://repositorio.usil.edu.pe/server/api/core/bitstreams/b88e8262-a3a3-411f-b89c-7d7014fa9a7a/content

- Zegarra Velasquez, R. L., Castillo Guerrero, H. H., Bianchi 
Rojas, A. J., & Muñoz Ruiz, V. P. (2022). Propuesta de uso de bicicletas en Lima Metropolitana como alternativa contra el caos vehicular. [Tesis de maestría, Pontificia Universidad Católica del Perú]. http://hdl.handle.net/20.500.12404/22044 

## Anexos

**Anexo 1:**
Presentación del Proyecto: https://www.canva.com/design/DAGCVM1sXj4/VNYTMKRbAUu-4MwGJqEtBA/edit?utm_content=DAGCVM1sXj4&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

**Anexo 2:**
Landing Page:<br> https://upc-pre-202401-si720-si91-ruedarent.github.io/Ruedarent-Landing-Page/

**Anexo 3:**
Web Applications Mock-ups: https://www.figma.com/file/WATKX4mlDctquazhZwgUB9/mockups?type=design&node-id=0%3A1&mode=design&t=oV4ZYw2Es2V34LBK-1 
