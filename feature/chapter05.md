## **Capítulo V: Product Implementation, Validation & Deployment
### 5.1. Software Configuration Management.
#### 5.1.1. Software Development Environment Configuration.
En esta sección especificaremos y detallaremos las plataformas y software que usamos como equipo para la realización de nuestro startup.

- GitHub: En esta plataforma es donde crearemos nuestro repositorio donde realizaremos los avances de nuestro startup. Además, nos ayuda a tener un mejor control en el trabajo de equipo debido a que se puede visualizar el avance de cada integrante a través de los commits.

https://github.com

- Whatsapp: Es una aplicación de mensajería instantánea multiplataforma que permite a los usuarios enviar mensajes de texto, voz y multimedia, así como realizar llamadas y videollamadas gratuitas a través de una conexión a Internet. Con una interfaz intuitiva y amplia disponibilidad en dispositivos móviles y de escritorio, WhatsApp se ha convertido en una herramienta omnipresente para la comunicación personal y empresarial en todo el mundo.

https://whatsapp.com/


- Visual Studio Code: Es un editor de código fuente ligero pero potente, desarrollado por Microsoft, que ofrece una amplia gama de características para programadores. Con soporte para múltiples lenguajes de programación, extensiones personalizables, integración con control de versiones y depuración, así como una interfaz intuitiva y altamente personalizable, Visual Studio Code se ha convertido en una opción popular para desarrolladores de software en todo el mundo.

https://code.visualstudio.com/

- Git: Sistema de control de versiones más usado, es un requisito para poder realizar los commits en Github.

https://git-scm.com/downloads

#### 5.1.2. Source Code Management.

##### Gestión del Código Fuente: 
En esta sección, explicaremos cómo gestionamos y seguimos el desarrollo del código en Ruedarent. Utilizamos GitHub como plataforma y Git como sistema de control de versiones.

Repositorio en GitHub para el Landing Page: https://github.com/upc-pre-202401-si720-si91-Ruedarent/Ruedarent-Landing-Page

##### Repositorio en GitHub para el registro de acceptance test files:
##### Metodología de Ramas:
En Ruedarent, implementamos el flujo de trabajo GitFlow para el control de versiones. Este flujo consta de varias ramas clave:
- Rama Principal (Main): Es la rama principal y raíz de nuestro desarrollo. Aquí se refleja el estado actual del código fuente y se redirige a producción. Cada vez que finalizamos tareas en otras ramas, se incorporan al producto final a través de esta rama.
- Rama de Desarrollo (Develop): Esta rama contiene el código fuente más reciente en desarrollo. Todos los cambios que están listos para publicarse se fusionan en la rama principal (Main) con una etiqueta de versión. Los cambios en esta rama se vuelven a fusionar en la rama principal para reflejar una nueva versión del producto.
- Ramas de Funcionalidad (Feature Branches): Utilizamos estas ramas para desarrollar nuevas características para las próximas versiones de TeachAid. Se ramifican desde la rama de desarrollo (Develop) y, una vez que el desarrollo está completo, se fusionan nuevamente en la rama de desarrollo o se descartan si la función no es exitosa.
- Ramas de Lanzamiento (Release Branches): Estas ramas nos permiten preparar el proyecto final para pruebas finales y correcciones de errores. Se ramifican desde la rama de desarrollo (Develop) y se fusionan nuevamente en esta para reflejar la "próxima versión". Seguimos convenciones específicas para nombrar nuestras ramas de lanzamiento.
- Ramas de Corrección Urgente (Hotfix Branches): Estas ramas se utilizan para resolver errores críticos de manera inmediata y preparar nuevas versiones del producto. Se ramifican desde la rama principal (Main) y se fusionan nuevamente en esta.

##### - Commits Convencionales:
En Ruedarent, seguimos la convención de commits convencionales para nuestros mensajes de confirmación. Estos mensajes siguen una estructura específica: 

- `<tipo>[ámbito opcional]: <descripción>` con opciones para el cuerpo y el pie del mensaje.
- Tipo "fix": Utilizamos este tipo de commit cuando se soluciona un error que afecta a los usuarios.
- Tipo "feat": Utilizamos este tipo de commit cuando se agrega una nueva característica para los usuarios.
- "BREAKING CHANGE": Utilizamos esta etiqueta en el pie del mensaje para comunicar cambios significativos en la API.

También se permiten otros tipos de commits, como "perf" (rendimiento), "build" (cambios en la 
compilación), "docs" (cambios en la documentación), "refactor" (refactorización), "style" (cambios de
formato), "test" (agregar o refactorizar pruebas), entre otros.<br>

Estas prácticas nos ayudan a mantener un control efectivo del desarrollo de Ruedarent y a comunicar 
claramente los cambios en nuestro código fuente.

#### 5.1.3. Source Code Style Guide & Conventions.

##### Archivos Feature:
En nuestro proyecto, emplearemos el lenguaje Gherkin para definir y comprender nuestras historias de usuario. Utilizaremos la estructura proporcionada que incluye los elementos: "Feature, Scenario, Given, When, Then y Examples".

- US01: 
- US02:
- US03:
- US04:
- US05:
#### 5.1.4. Software Deployment Configuration.
### 5.2. Landing Page, Services & Applications Implementation.
#### 5.2.1. Sprint 1
#### 5.2.1.1. Sprint Planning 1.
#### 5.2.1.2. Sprint Backlog 1.
#### 5.2.1.3. Development Evidence for Sprint Review.


#### 5.2.1.4. Testing Suite Evidence for Sprint Review.
#### 5.2.1.5. Execution Evidence for Sprint Review.
#### 5.2.1.6. Services Documentation Evidence for Sprint Review.
#### 5.2.1.7. Software Deployment Evidence for Sprint Review.
#### 5.2.1.8. Team Collaboration Insights during Sprint.
## Concluciones
## Bibliografía
## Anexos