# Instalación de Maven en el SO

## 1.- Instalar Apache Maven

Primero actualizamos los repositorios de Ubuntu:

<img src="img/01.png">

Instalamos Maven:

<img src="img/02.png">

Verificamos la versión instalada:

<img src="img/03.png">

Vemos que se descarga la versión 3.6.3, pero la última versión es la 3.8.2 por lo que necesitamos instalar la versión concreta de Maven.

## 2.- Instalar una versión concreta de Apache Maven

Descargamos la versión 3.8.2 en el directorio /tmp:

<img src="img/04.png">

Una vez completada la descarga, extraemos los archivos en el directorio /opt:

<img src="img/05.png">

Ahora creamos un enlace simbólico que apunte al directorio de instalación de maven para tener más control sobre este:

<img src="img/06.png">

### 2.1.- Establecer variables de entorno

Creamos el archivo maven.sh en el directorio “/etc/profile.d” y lo abrimos con el editor nano:

<img src="img/07.png">

Añadimos el siguiente código:

<img src="img/08.png">

Guardamos el archivo y le damos permisos de ejecució:

<img src="img/09.png">

Finalmente, cargamos las variables de entorno usando el comando source.

<img src="img/10.png">

### 2.2.- Verificar la instalación

Ejecutamos el comando “mvn -version” y vemos que ahora sí aparece la versión actual de Apache Maven.

<img src="img/11.png">
