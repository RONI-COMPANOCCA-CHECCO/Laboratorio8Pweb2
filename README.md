<div align="center">
<table>
    <theader>
        <tr>
            <td><img src="https://github.com/rescobedoq/pw2/blob/main/epis.png?raw=true" alt="EPIS" style="width:50%; height:auto"/></td>
            <th>
                <span style="font-weight:bold;">UNIVERSIDAD NACIONAL DE SAN AGUSTIN</span><br />
                <span style="font-weight:bold;">FACULTAD DE INGENIERÍA DE PRODUCCIÓN Y SERVICIOS</span><br />
                <span style="font-weight:bold;">DEPARTAMENTO ACADÉMICO DE INGENIERÍA DE SISTEMAS E INFORMÁTICA</span><br />
                <span style="font-weight:bold;">ESCUELA PROFESIONAL DE INGENIERÍA DE SISTEMAS</span>
            </th>
            <td><img src="https://github.com/rescobedoq/pw2/blob/main/abet.png?raw=true" alt="ABET" style="width:50%; height:auto"/></td>
        </tr>
    </theader>
    <tbody>
        <tr><td colspan="3"><span style="font-weight:bold;">Formato</span>: Guía de Práctica de Laboratorio</td></tr>
        <tr><td><span style="font-weight:bold;">Aprobación</span>:  2023/02/01</td><td><span style="font-weight:bold;">Código</span>: GUIA-PRLD-001</td><td><span style="font-weight:bold;">Página</span>: 1</td></tr>
    </tbody>
</table>
</div>

<div align="center">
<span style="font-weight:bold;">GUÍA DE LABORATORIO</span><br />
</div>


<table>
<theader>
<tr><th colspan="6">INFORMACIÓN BÁSICA</th></tr>
</theader>
<tbody>
<tr><td>ASIGNATURA:</td><td colspan="5">Programación Web 2</td></tr>
<tr><td>TÍTULO DE LA PRÁCTICA:</td><td colspan="5">Django Rest Framework</td></tr>
<tr>
<td>NÚMERO DE PRÁCTICA:</td><td>08</td><td>AÑO LECTIVO:</td><td>2023 A</td><td>NRO. SEMESTRE:</td><td>III</td>
</tr>
<tr>
<td>FECHA INICIO::</td><td>18-Jul-2023</td><td>FECHA FIN:</td><td>25-Jul-2023</td><td>DURACIÓN:</td><td>04 horas</td>
</tr>
<tr><td colspan="6">RECURSOS:
    <ul>
        <li>https://www.w3schools.com/python/python_reference.asp</li>
        <li>https://docs.python.org/3/tutorial/</li>
        <li>https://developer.mozilla.org/es/docs/Learn/Server-side/Django/Models</li>
        <li>https://tutorial.djangogirls.org/es/django_models/</li>
        <li>https://pear.php.net/manual/en/standards.php</li>
        <li>https://docs.djangoproject.com/en/4.0/</li>
        <li>https://www.youtube.com/watch?v=M4NIs4BM1dk</li>
        <li>https://pypi.org/</li>
        <li>https://pip.pypa.io/en/latest/user_guide/</li>
        <li>https://packaging.python.org/en/latest/tutorials/installing-packages/</li>
    </ul>
</td>
</<tr>
<tr><td colspan="6">DOCENTE:
<ul>
<li>Ing. Anibal Sardon</li>
</ul>
</td>
</<tr>
<tr><td colspan="6">ALUMNO:
<ul>
<li>Roni Companocca Checco</li>
</ul>
</td>
</<tr>
<tr><td colspan="6">LINK REPOSITORIO:
<ul>
<li>https://github.com/RONI-COMPANOCCA-CHECCO/Laboratorio8Pweb2.git</li>
</ul>
</td>
</<tr>
</tdbody>
</table>

# Django

[![License][license]][license-file]
[![Downloads][downloads]][releases]
[![Last Commit][last-commit]][releases]

[![Debian][Debian]][debian-site]
[![Git][Git]][git-site]
[![GitHub][GitHub]][github-site]
[![Vim][Vim]][vim-site]
[![Java][Java]][java-site]

#

## 1. Competencias del curso

- General: C.c. Dise ̃na responsablemente aplicaciones web, sus componentes o procesos para satisfacer necesidades dentro de restricciones realistas: econ ́omicas, medio ambientales, sociales, políticas,  ́eticas, de salud, de seguridad, manufacturación y sostenibilidad.

- Específica: C.m. Construye responsablemente soluciones con tecnolog ́ıa web siguiendo un proceso adecuado llevando a cabo las pruebas ajustada a los recursos disponibles del cliente.

- Específica: C.p. Aplica de forma flexible técnicas, métodos, principios, normas, estándares y herramientas del desarrollo web necesarias para la construcción de aplicaciones web e implementación de estos sistemas en una organización.

## 2. Resultado del estudiante

- RE. 2 La capacidad de aplicar diseño de ingeniería para producir soluciones a problemas y diseñar sistemas, componentes o procesos para satisfacer necesidades espec ́ıficas dentro de consideraciones realistas en los aspectos de salud pública, seguridad y bienestar; factores globales, culturales, sociales, económicos y ambientales.

- RE. 8 La capacidad de crear, seleccionar y utilizar t ́ecnicas, habilidades, recursos y herramientas modernas de ingeniería y tecnologías de la información, incluyendo la predicción y el modelamiento, con una comprensión de las limitaciones.

## 3. Equipos, materiales y temas

- Sistema Operativo (GNU/Linux de preferencia).
- GNU Vim.
- Python 3.
- Git.
- Cuenta en GitHub con el correo institucional.
- Entorno virtual.
- Django 4.
- djangorestframework.

## 4. Directorio de trabajo

- Cree su directorio de trabajo.
- Luego, dir ́ıjase a este directorio, para clonar su repositorio y continuar sus practicas.

             Listing 1: Creando directorio de trabajo

        $ mkdir -p $HOME/rescobedoq/


             Listing 2: Dirij ́ıendonos al directorio de trabajo

        $ cd $HOME/rescobedoq/


             Listing 3: Clonando repositorio GitHub

        $ git clone [URL_DE_SU_GITHUB_PRIVADO]


             Listing 4: Creando directorio para laboratorio
        $ mkdir -p $HOME/rescobedoq/pw2-lab-23a/lab07/exercises/


- Siempre evalue utilizar el archivo .gitignore para no considerar algunos archivo innecesarios sobre todo para el repositorio GitHub.
- Pueden haber varios de estos archivos y estar ubicados estrat ́egicamente; por ejemplo s ́olo para un laboratorio en particular.

             Listing 5: Creando .gitignore
        $ vim $HOME/rescobedoq/pw2-lab-23a/lab07/.
        

             Listing 6: Ejemplo de .gitignore
        my_env/bin/*
        my_env/lib/*
        my_env/src/__pycache__/*
        *.pyc


- Estudie el archivo .gitignore del proyecto Library :
- https://github.com/mdn/django-locallibrary-tutorial/blob/main/.gitignore


## 5. Marco teórico

### 5.1. Django Rest Framework

- Django REST framework es un conjunto de herramientas potente y flexible para crear API web.
- Algunas razones por las que podr ́ıa querer usar el marco REST:
  - La API navegable por la Web es una gran ganancia de usabilidad para sus desarrolladores.
  - Pol ́ıticas de autenticaci ́on que incluyen paquetes para OAuth1 y OAuth2.
  - Serializaci ́on que admite fuentes de datos ORM y no ORM.
  - Personalizable hasta el final: solo use las vistas regulares basadas en funciones si no necesita las funciones m ́as potentes .
  - Amplia documentaci ́on y gran apoyo de la comunidad .
  - Utilizado y confiado por empresas reconocidas internacionalmente, como Mozilla, Red Hat, Heroku y Eventbrite.

### 5.2. Crear un directorio para el entorno virtual de Django

- Para crear un ambiente elija en qu ́e directorio se va crear el entorno virtual.
- No env ́ıe estos entornos virtuales al GitHub, om ́ıtalos en .gitignore. Pero no olvide tener requirements.txt en el root del Proyecto.

             Listing 7: Creando directorio para entorno virtual en Unix

        $ mkdir -p $HOME/rescobedoq/pw2-lab-23a/lab07/my_env

### 5.3. Crear entorno virtual en un directorio

- En este directorio crear un entorno virtual ejecutando el siguiente comando:

             Listing 8: Creando entorno virtual en GNU/Linux

        $ cd $HOME/rescobedoq/pw2-lab-23a/lab07/my_env
        $ virtualenv -p python3 .


             Listing 9: Creando entorno virtual en MS Windows

        C:\>python -m venv c:\rescobedoq\pw2-lab-23a\lab07\my_env
 
  
             Listing 10: Creando entorno virtual en MacOS

        $ python -m venv $HOME/rescobedoq/pw2-lab-23a/lab07/my_env

### 5.4. Activando entorno virtual

- En el directorio de trabajo active el entorno virtual ejecutando el script activate. Sea cual sea nuestro sistema operativo sabremos que el entorno virtual se ha activado porque su
- nombre aparece entre par ́entesis delante del promt.

             Listing 11: Activando entorno virtual en GNU/Linux

        $ cd $HOME/rescobedoq/pw2-lab-23a/lab07/exercises/
        $ source ./../my_env/bin/activate
        (my_env) user@localhost:$


             Listing 12: Activando entorno virtual en MS Windows
        C:\rescobedoq\pw2-lab-23a\lab07\my_env\scripts\activate.bat
        Listing 13: Activando entorno virtual en GNU/Linux
        $ source $HOME/rescobedoq/pw2-lab-23a/lab07/my_env/bin/activate

### 5.5. Desactivando entorno virtual

- El comando para desactivar el entorno virtual es id ́entico para Windows, macOS y Linux:

             Listing 14: Desactivando entorno virtual

        $ deactivate

### 5.6. Instalando Django y Django Rest Framework dentro del entorno virtual

- Requisitos.
- El framework REST requiere lo siguiente:
  - Python (3.6, 3.7, 3.8, 3.9, 3.10)
  - Django (2.2, 3.0, 3.1, 3.2, 4.0, 4.1)
- Recomendamos encarecidamente y solo admitimos oficialmente la  ́ultima versi ́on del parche de cada serie de Python y Django.
- Los siguientes paquetes son opcionales:
  - PyYAML , uritemplate (5.1+, 3.0.0+) : Compatibilidad con la generaci ́on de esquemas.
  - Markdown (3.0.0+) : compatibilidad con Markdown para la API navegable.
  - Pygments (2.4.0+) : agregue resaltado de sintaxis al procesamiento de Markdown.
  - django-filter (1.0.1+) : Soporte de filtrado.
  - django-guardian (1.1.1+) : Soporte de permisos de nivel de objeto.

             Listing 15: Mostrando paquetes instalados en el entorno virtual

        (my_env) user@localhost:$ pip list
        Package Version
        ---------- -------
        pip 22.0.4
        setuptools 62.1.0
        wheel 0.37.1


- Instalamos con pip: (Puede incluir los paquetes opcionales que desee)

             Listing 16: Instando Django

        (my_env) user@localhost:$ pip install django
        (my_env) user@localhost:$ pip install djangorestframework
        (my_env) user@localhost:$ pip install markdown
        (my_env) user@localhost:$ pip install django-filter

- Volvemos a listar los paquetes instalados:

             Listing 17: Mostrando Django instalado en el entorno virtual

        (my_env) user@localhost:$ pip list
        Package Version
        ------------------- -------
        asgiref 3.7.2
        Django 4.2.3
        django-filter 23.2
        djangorestframework 3.14.0
        Markdown 3.4.3
        pip 23.0.1
        pytz 2023.3
        setuptools 66.1.1
        sqlparse 0.4.4
        wheel 0.38.4


- Importante: Como el entorno virtual no se clona, por temas de espacio. Es necesario sacarle un backup en un arquivo requirements.txt

             Listing 18: Creando requirements.txt

        (my_env) user@localhost:$ pip freeze > requirements.txt
        Importante: El arquivo requirements.txt, servir ́a para volver a construir el entorno
        virtual, preservando los paquetes con sus versiones.


             Listing 19: Instalando desde requirements.txt

        (my_env) user@localhost:$ pip install -r requirements.txt

## 6. Ejercicios

- Practique desarrollando el ejercicio de iniciaci ́on:
- https://www.django-rest-framework.org/tutorial/quickstart/
- Para consumir el web-service puede usar el cliente SOAP UI Community: https://www.soapui.org/downloads/soapui/

## 7. Tarea

- En sus grupos de trabajo correspondientes. Elabore un servicio web que tenga un CRUD con el uso de este framework.
- Create - POST
- Read - GET
- Update - PUT
- Delete - DELETE
- Centrarce en el Core business de su aplicaci ́on web. Los m ́as importante y necesario que este disponible a traves de un servicio web.
- Ejemplos: https://reqbin.com/, https://www.googleapis.com/youtube/v3/playlistItems
- Muestre la funcionalidad consumiendola desde el cliente Rest de su preferencia.
- El m ́etodo GET puede ser directamente consumido por un navegador web:
- Por ejemplo: En esta API se puede obtener la temperatura de Arequipa en un rango de fechas: (La versi ́on gratuita tiene un retraso de 7 d ́ıas, por tanto s ́olo mostrar ́a la temperatura en Arequipa desde el 01 de Julio hasta el 03 de Julio)
- https://archive-api.open-meteo.com/v1/archive?latitude=-16.39889&longitude=-71.535&start_date=2023-07-01&end_date=2023-07-10&hourly=temperature_2m&daily=temperature_2m_max,temperature_2m_min&timezone=America%2FNew_York

## 8. Pregunta

- ¿Cu ́al fu ́e la mayor dificultad del uso de este framework?.

## 9. Entregables

- El informe debe tener un enlace al directorio espec ́ıfico del laboratorio en su repositorio GitHub privado donde est ́e todo el c ́odigo fuente y otros que sean necesarios. Evitar la presencia de archivos: binarios, objetos, archivos temporales, cache, librerias, entornos virtuales. Si hay configuraciones particulares puede incluir archivos de especificaci ́on como: requirements.txt, o leeme.txt.
- No olvide que el profesor debe ser siempre colaborador a su repositorio (Usuario del profesor @rescobedoq).
- Para ser considerado con la calificaci ́on de m ́axima nota, el informe debe estar elab ́orado en LATEX
- Usted debe describir s ́olo los commits m ́as importantes que marcaron hitos en su trabajo, adjutando capturas de pantalla, del commit, del c ́odigo fuente, de sus ejecuciones y pruebas.
- En el informe siempre se debe explicar las im ́agenes (c ́odigo fuente, capturas de pantalla, commits, ejecuciones, pruebas, etc.) con descripciones puntuales pero precisas.
- Partes de entrega:
  - Django orientado a Usuarios finales.
  - Tema para clientes, con funcionalidades importantes.
  - Recomendaciones: CRUD en uno de los procesos para el cliente final.
  - Ejemplo 1: Para la WebApp Library (Sistema de Biblioteca virtual), ser ́ıa .El cliente reserva un ejemplar de un libro determinado”.
  - Ejemplo 2: Para la WebApp Enrollments (Sistema para Inscripciones en laboratorios), ser ́ıa El alumno se inscribe en un laboratorio disponible para un curso”.

## 10. R ́ubricas

### 10.1. R ́ubrica para entregable Informe

***Tabla 1: R ́ubrica para tipo de Informe***

<a href="https://ibb.co/ChdDQ4t"><img src="https://i.ibb.co/f4RLHZS/tabla1.jpg" alt="tabla1" border="0"></a>

### 10.2. R ́ubrica para el contenido del Informe y demostraci ́on

- El alumno deber ́a marcar o dejar en blanco en las celdas de la columna Checklist, deacuerdo asi cumpli ́o o no con el  ́ıtem correspondiente.
- Si un alumno supera la fecha de entrega, su calificaci ́on siempre ser ́a sobre la nota m ́ınima aprobada, siempre y cuando cumpla con todos lo items.
- El alumno debe autocalificarse en la columna Estudiante de acuerdo a la tabla de calificaci ́on de niveles de desempe ̃no:

***Tabla 2: Niveles de desempe ̃no***

<a href="https://imgbb.com/"><img src="https://i.ibb.co/4Z9FBmy/tabla2.jpg" alt="tabla2" border="0"></a>

***Tabla 3: R ́ubrica para contenido del Informe y demostraci ́on***

<a href="https://ibb.co/x7tyPM0"><img src="https://i.ibb.co/rwRgTZS/tabla-3-2.jpg" alt="tabla-3-2" border="0"></a>

## 6. Referencias

- https://www.django-rest-framework.org/
- https://www.django-rest-framework.org/tutorial/quickstart/
- https://www.django-rest-framework.org/tutorial/1-serialization/
- https://www.django-rest-framework.org/tutorial/3-class-based-views/
- https://www.django-rest-framework.org/api-guide/authentication/
- https://www.bezkoder.com/django-rest-api/
- https://stackoverflow.com/questions/70319606/importerror-cannot-import-name-url-from-django-conf-urls-after-upgrading-to
#

[license]: https://img.shields.io/github/license/rescobedoq/pw2?label=rescobedoq
[license-file]: https://github.com/rescobedoq/pw2/blob/main/LICENSE

[downloads]: https://img.shields.io/github/downloads/rescobedoq/pw2/total?label=Downloads
[releases]: https://github.com/rescobedoq/pw2/releases/

[last-commit]: https://img.shields.io/github/last-commit/rescobedoq/pw2?label=Last%20Commit

[Debian]: https://img.shields.io/badge/Debian-D70A53?style=for-the-badge&logo=debian&logoColor=white
[debian-site]: https://www.debian.org/index.es.html

[Git]: https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white
[git-site]: https://git-scm.com/

[GitHub]: https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white
[github-site]: https://github.com/

[Vim]: https://img.shields.io/badge/VIM-%2311AB00.svg?style=for-the-badge&logo=vim&logoColor=white
[vim-site]: https://www.vim.org/

[Java]: https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=java&logoColor=white
[java-site]: https://docs.oracle.com/javase/tutorial/


[![Debian][Debian]][debian-site]
[![Git][Git]][git-site]
[![GitHub][GitHub]][github-site]
[![Vim][Vim]][vim-site]
[![Java][Java]][java-site]


[![License][license]][license-file]
[![Downloads][downloads]][releases]
[![Last Commit][last-commit]][releases]
