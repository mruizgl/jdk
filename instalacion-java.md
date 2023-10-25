<div>

# Instalación de JDK en Linux
## Introducción
Vamos a instalar Java con el JDK el cual es un entorno de desarrollo y el entorno de ejecución JRE. También aprenderemos a movernos en sus diferentes versiones en función de nuestras necesidades, pero antes vamos a hablar sobre qué es Java.
### ¿Qué es Java?
Java es un lenguaje de programación creada por Sun Microsystems en 1995. Ha evolucionado desde sus humildes comienzos hasta impulsar una gran parte del mundo digital actual, ya que es una plataforma fiable en la que se crean muchos servicios y aplicaciones.   
### ¿Cómo instalar Java en Linux desde repositorios?
Lo primero debemos de actualizar el sistema ejecutando en el termina del S.O. el siguiente comando. Nos solicitará la contraseña del admin, la metemos y se actualiza el sistema.

```
sudo apt-get update
```

EJECUCIÓN EN MI TERMINAL:

```

melissa@melissa-linux:~$ sudo apt-get update
Obj:1 http://archive.ubuntu.com/ubuntu jammy InRelease
Des:2 http://security.ubuntu.com/ubuntu jammy-security InRelease [110 kB]      
Des:3 http://archive.ubuntu.com/ubuntu jammy-updates InRelease [119 kB]        
Ign:4 http://packages.linuxmint.com victoria InRelease                         
Des:5 http://archive.ubuntu.com/ubuntu jammy-backports InRelease [109 kB]
Des:6 http://packages.linuxmint.com victoria Release [24,2 kB]
Des:7 http://security.ubuntu.com/ubuntu jammy-security/main i386 Packages [353 kB]
Des:8 http://archive.ubuntu.com/ubuntu jammy-updates/main i386 Packages [515 kB]
Des:9 http://packages.linuxmint.com victoria Release.gpg [833 B]               
Des:10 http://security.ubuntu.com/ubuntu jammy-security/main amd64 Packages [896 kB]
Des:11 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 Packages [1.103 kB]
Des:12 http://security.ubuntu.com/ubuntu jammy-security/main amd64 DEP-11 Metadata [43,0 kB]
Des:13 http://security.ubuntu.com/ubuntu jammy-security/main amd64 c-n-f Metadata [11,4 kB]
Des:14 http://security.ubuntu.com/ubuntu jammy-security/universe amd64 Packages [793 kB]
Des:15 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 DEP-11 Metadata [101 kB]
Des:16 http://security.ubuntu.com/ubuntu jammy-security/universe amd64 DEP-11 Metadata [55,1 kB]
Des:17 http://security.ubuntu.com/ubuntu jammy-security/universe amd64 c-n-f Metadata [16,8 kB]
Des:18 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 c-n-f Metadata [16,0 kB]
Des:19 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 Packages [995 kB]
Des:20 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 DEP-11 Metadata [305 kB]
Des:21 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 c-n-f Metadata [22,0 kB]
Des:22 http://archive.ubuntu.com/ubuntu jammy-updates/multiverse amd64 DEP-11 Metadata [940 B]
Des:23 http://archive.ubuntu.com/ubuntu jammy-backports/main amd64 DEP-11 Metadata [4.920 B]
Des:24 http://archive.ubuntu.com/ubuntu jammy-backports/universe amd64 DEP-11 Metadata [17,9 kB]
Des:25 http://packages.linuxmint.com victoria/upstream amd64 Packages [48,4 kB]
Descargados 5.659 kB en 3s (2.224 kB/s)
Leyendo lista de paquetes... Hecho

```

------

A continuación instalamos Java con el siguiente comando
```
sudo apt-get install default-jdk
``` 
EJECUCIÓN EN MI TERMINAL:

```
melissa@melissa-linux:~$ sudo apt-get install default-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
Configurando libpthread-stubs0-dev:amd64 (0.4-1build2) ...
Configurando xtrans-dev (1.4.0-1) ...
Configurando default-jdk-headless (2:1.11-72build2) ...
Configurando openjdk-11-jdk:amd64 (11.0.20.1+1-0ubuntu1~22.04) ...
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jconsole para proveer /usr/bin/jconsole (jconsole) en modo automático
Configurando xorg-sgml-doctools (1:1.11-1.1) ...
Configurando default-jdk (2:1.11-72build2) ...
Procesando disparadores para sgml-base (1.30) ...
Procesando disparadores para mailcap (3.70+nmu1ubuntu1) ...
Configurando x11proto-dev (2021.5-1) ...
Procesando disparadores para desktop-file-utils (0.26+mint3+victoria) ...
Configurando libxau-dev:amd64 (1:1.0.9-1build5) ...
Procesando disparadores para hicolor-icon-theme (0.17-2) ...
Configurando libice-dev:amd64 (2:1.0.10-1build2) ...
Procesando disparadores para gnome-menus (3.36.0-1ubuntu3) ...
Configurando libsm-dev:amd64 (2:1.2.3-1build2) ...
Procesando disparadores para libc-bin (2.35-0ubuntu3.1) ...
Procesando disparadores para man-db (2.10.2-1) ...
Configurando libxdmcp-dev:amd64 (1:1.1.3-0ubuntu5) ...
Configurando libxcb1-dev:amd64 (1.14-3ubuntu3) ...
Configurando libx11-dev:amd64 (2:1.7.5-1ubuntu0.3) ...
Configurando libxt-dev:amd64 (1:1.2.1-1) ...

```

---------

Listamos versión que tenemos de Java con el siguiente comando: 

```
java --version
```
EJECUCIÓN EN MI TERMINAL:

```
melissa@melissa-linux:~$ java --version
openjdk 11.0.20.1 2023-08-24
OpenJDK Runtime Environment (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04)
OpenJDK 64-Bit Server VM (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04, mixed mode, sharing)

```


--------


## ¿Cómo instalar una versión específica de Java? 
Para instalar Open JDK 11
```
sudo apt install openjdk-11-jdk
```
EJECUCIÓN EN MI TERMINAL:
```
melissa@melissa-linux:~$ sudo apt install openjdk-11-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
openjdk-11-jdk ya está en su versión más reciente (11.0.20.1+1-0ubuntu1~22.04).
fijado openjdk-11-jdk como instalado manualmente.
0 actualizados, 0 nuevos se instalarán, 0 para eliminar y 204 no actualizados.
```

-----

Para instalar 13
```
sudo apt install openjdk-13-jdk
```
EJECUCIÓN EN MI TERMINAL:
```
melissa@melissa-linux:~$ sudo apt install openjdk-13-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
E: No se ha podido localizar el paquete openjdk-13-jdk
```

-----
Para instalar 8 
```
sudo apt install openjdk-8-jdk
```
EJECUCIÓN EN MI TERMINAL:

```
melissa@melissa-linux:~$ sudo apt install openjdk-8-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho

update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/wsgen para
 proveer /usr/bin/wsgen (wsgen) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/wsimport p
ara proveer /usr/bin/wsimport (wsimport) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/xjc para p
roveer /usr/bin/xjc (xjc) en modo automático
Configurando openjdk-8-jre:amd64 (8u382-ga-1~22.04.1) ...
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/policy
tool para proveer /usr/bin/policytool (policytool) en modo automático
Configurando openjdk-8-jdk:amd64 (8u382-ga-1~22.04.1) ...
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/appletview
er para proveer /usr/bin/appletviewer (appletviewer) en modo automático
Procesando disparadores para fontconfig (2.13.1-4.2ubuntu5) ...
Procesando disparadores para desktop-file-utils (0.26+mint3+victoria) ...
Procesando disparadores para hicolor-icon-theme (0.17-2) ...
Procesando disparadores para gnome-menus (3.36.0-1ubuntu3) ...
Procesando disparadores para libc-bin (2.35-0ubuntu3.1) ...
Procesando disparadores para mailcap (3.70+nmu1ubuntu1) ...

```

----

La version que se debe trabajar es la version 8. Para ello verificaremos la version de java que se esta ejecutando: 
```
java --version
```
EJECUCIÓN EN MI TERMINAL:

```
melissa@melissa-linux:~$ java --version
openjdk 11.0.20.1 2023-08-24
OpenJDK Runtime Environment (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04)
OpenJDK 64-Bit Server VM (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04, mixed mode, sharing)

```

----

Como podemos observar tenemos la version 11, debemos configurar las variables de entorno para ponerla en la 8 que es con lo que vamos a trabajar.

## Configuración de variables de entorno

El siguiente paso consiste en establecer las variables de entorno. Es necesario porque cuando se usa Java, Linux necesita saber dónde está ubicado el programa para ejecutarlo y qué versión de Java usar de forma predeterminada.

### Listar las versiones de OpenJDK instaladas
Para ello utilizaremos 
```
 ls /usr/lib/jvm
```

### Actualización de variables de entorno
Edita y modifica el fichero profile, con los comandos: 
```
sudo update-alternatives --config java
```
Selecciona el que desees. En mi caso se verá en el output de abajo que selecciono la versión 8.

EJECUCIÓN EN MI TERMINAL:

```
melissa@melissa-linux:~$ sudo update-alternatives --config java
Existen 2 opciones para la alternativa java (que provee /usr/bin/java).

  Selección   Ruta                                            Prioridad  Estado
------------------------------------------------------------
  0            /usr/lib/jvm/java-11-openjdk-amd64/bin/java      1111      modo automático
  1            /usr/lib/jvm/java-11-openjdk-amd64/bin/java      1111      modo manual
* 2            /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java   1081      modo manual

Pulse <Intro> para mantener el valor por omisión [*] o pulse un número de selección: 2
```

----

Otra opcion es añadir el siguiente código
```
# Java version
JAVA_HOME=/usr/lib/jvm/(SELECCIONA UN PATH DE LA VERSION QUE DESEAS QUE SE EJECUTE)
PATH=$PATH:$HOME/bin:$JAVA_HOME/bin
export JAVA_HOME
export JRE_HOME
export PATH
```
en 
```
/etc/profile.d/java.sh
```
Hacemos el script ejecutable con el siguiente comando: 
```
sudo chmod +x /etc/profile.d/java.sh
```
Finalmente, cargue las variables de entorno usando el comando de source
```
source /etc/profile.d/java.sh
```
</div>
