<div>

# Instalación de JDK en Linux
## Introducción
Vamos a instalar Java con el JDK el cual es un entorno de desarrollo y el entorno de ejecución JRE. También aprenderemos a movernos en sus diferentes versiones en función de nuestras necesidades, pero antes vamos a hablar sobre qué es Java.
### ¿Qué es Java?
Java es un lenguaje de programación creada por Sun Microsystems en 1995. Ha evolucionado desde sus humildes comienzos hasta impulsar una gran parte del mundo digital actual, ya que es una plataforma fiable en la que se crean muchos servicios y aplicaciones.   
### ¿Cómo instalar Java en Linux desde repositorios?
Lo primero debemos de actualizar el sistema ejecutando en el termina del S.O. el siguiente comando. Nos solicitará la contraseña del admin, la metemos y se actualiza el sistema.

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

A continuación instalamos Java con el siguiente comando 
```
melissa@melissa-linux:~$ sudo apt-get install default-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
Se instalarán los siguientes paquetes adicionales:
  default-jdk-headless libice-dev libpthread-stubs0-dev libsm-dev libx11-6
  libx11-dev libx11-xcb1 libxau-dev libxcb1-dev libxdmcp-dev libxt-dev
  openjdk-11-jdk openjdk-11-jdk-headless openjdk-11-jre
  openjdk-11-jre-headless x11proto-dev xorg-sgml-doctools xtrans-dev
Paquetes sugeridos:
  libice-doc libsm-doc libx11-doc libxcb-doc libxt-doc openjdk-11-demo
  openjdk-11-source visualvm fonts-dejavu-extra fonts-ipafont-gothic
  fonts-ipafont-mincho fonts-wqy-microhei | fonts-wqy-zenhei
Paquetes recomendados:
  libatk-wrapper-java-jni fonts-dejavu-extra
Se instalarán los siguientes paquetes NUEVOS:
  default-jdk default-jdk-headless libice-dev libpthread-stubs0-dev libsm-dev
  libx11-dev libxau-dev libxcb1-dev libxdmcp-dev libxt-dev openjdk-11-jdk
  openjdk-11-jdk-headless x11proto-dev xorg-sgml-doctools xtrans-dev
Se actualizarán los siguientes paquetes:
  libx11-6 libx11-xcb1 openjdk-11-jre openjdk-11-jre-headless
4 actualizados, 15 nuevos se instalarán, 0 para eliminar y 204 no actualizados.
Se necesita descargar 120 MB de archivos.
Se utilizarán 90,6 MB de espacio de disco adicional después de esta operación.
¿Desea continuar? [S/n] s
Des:1 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 libx11-6 amd64 2:1.7.5-1ubuntu0.3 [667 kB]
Des:2 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 libx11-xcb1 amd64 2:1.7.5-1ubuntu0.3 [7.802 B]
Des:3 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 openjdk-11-jre amd64 11.0.20.1+1-0ubuntu1~22.04 [213 kB]
Des:4 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 openjdk-11-jre-headless amd64 11.0.20.1+1-0ubuntu1~22.04 [42,5 MB]
Des:5 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 openjdk-11-jdk-headless amd64 11.0.20.1+1-0ubuntu1~22.04 [73,5 MB]
Des:6 http://archive.ubuntu.com/ubuntu jammy/main amd64 default-jdk-headless amd64 2:1.11-72build2 [942 B]
Des:7 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 openjdk-11-jdk amd64 11.0.20.1+1-0ubuntu1~22.04 [1.331 kB]
Des:8 http://archive.ubuntu.com/ubuntu jammy/main amd64 default-jdk amd64 2:1.11-72build2 [908 B]
Des:9 http://archive.ubuntu.com/ubuntu jammy/main amd64 xorg-sgml-doctools all 1:1.11-1.1 [10,9 kB]
Des:10 http://archive.ubuntu.com/ubuntu jammy/main amd64 x11proto-dev all 2021.5-1 [604 kB]
Des:11 http://archive.ubuntu.com/ubuntu jammy/main amd64 libice-dev amd64 2:1.0.10-1build2 [51,4 kB]
Des:12 http://archive.ubuntu.com/ubuntu jammy/main amd64 libpthread-stubs0-dev amd64 0.4-1build2 [5.516 B]
Des:13 http://archive.ubuntu.com/ubuntu jammy/main amd64 libsm-dev amd64 2:1.2.3-1build2 [18,1 kB]
Des:14 http://archive.ubuntu.com/ubuntu jammy/main amd64 libxau-dev amd64 1:1.0.9-1build5 [9.724 B]
Des:15 http://archive.ubuntu.com/ubuntu jammy/main amd64 libxdmcp-dev amd64 1:1.1.3-0ubuntu5 [26,5 kB]
Des:16 http://archive.ubuntu.com/ubuntu jammy/main amd64 xtrans-dev all 1.4.0-1 [68,9 kB]
Des:17 http://archive.ubuntu.com/ubuntu jammy/main amd64 libxcb1-dev amd64 1.14-3ubuntu3 [86,5 kB]
Des:18 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 libx11-dev amd64 2:1.7.5-1ubuntu0.3 [744 kB]
Des:19 http://archive.ubuntu.com/ubuntu jammy/main amd64 libxt-dev amd64 1:1.2.1-1 [396 kB]
Descargados 120 MB en 6s (21,6 MB/s)
(Leyendo la base de datos ... 527673 ficheros o directorios instalados actualmente.)
Preparando para desempaquetar .../libx11-6_2%3a1.7.5-1ubuntu0.3_amd64.deb ...
Desempaquetando libx11-6:amd64 (2:1.7.5-1ubuntu0.3) sobre (2:1.7.5-1ubuntu0.2) ...
Configurando libx11-6:amd64 (2:1.7.5-1ubuntu0.3) ...
(Leyendo la base de datos ... 527673 ficheros o directorios instalados actualmente.)
Preparando para desempaquetar .../00-libx11-xcb1_2%3a1.7.5-1ubuntu0.3_amd64.deb ...
Desempaquetando libx11-xcb1:amd64 (2:1.7.5-1ubuntu0.3) sobre (2:1.7.5-1ubuntu0.2) ...
Preparando para desempaquetar .../01-openjdk-11-jre_11.0.20.1+1-0ubuntu1~22.04_amd64.deb ...
Desempaquetando openjdk-11-jre:amd64 (11.0.20.1+1-0ubuntu1~22.04) sobre (11.0.19+7~us1-0ubuntu1~22.04.1) ...
Preparando para desempaquetar .../02-openjdk-11-jre-headless_11.0.20.1+1-0ubuntu1~22.04_amd64.deb ...
Desempaquetando openjdk-11-jre-headless:amd64 (11.0.20.1+1-0ubuntu1~22.04) sobre (11.0.19+7~us1-0ubuntu1~22.04.1) ...
Seleccionando el paquete openjdk-11-jdk-headless:amd64 previamente no seleccionado.
Preparando para desempaquetar .../03-openjdk-11-jdk-headless_11.0.20.1+1-0ubuntu1~22.04_amd64.deb ...
Desempaquetando openjdk-11-jdk-headless:amd64 (11.0.20.1+1-0ubuntu1~22.04) ...
Seleccionando el paquete default-jdk-headless previamente no seleccionado.
Preparando para desempaquetar .../04-default-jdk-headless_2%3a1.11-72build2_amd64.deb ...
Desempaquetando default-jdk-headless (2:1.11-72build2) ...
Seleccionando el paquete openjdk-11-jdk:amd64 previamente no seleccionado.
Preparando para desempaquetar .../05-openjdk-11-jdk_11.0.20.1+1-0ubuntu1~22.04_amd64.deb ...
Desempaquetando openjdk-11-jdk:amd64 (11.0.20.1+1-0ubuntu1~22.04) ...
Seleccionando el paquete default-jdk previamente no seleccionado.
Preparando para desempaquetar .../06-default-jdk_2%3a1.11-72build2_amd64.deb ...
Desempaquetando default-jdk (2:1.11-72build2) ...
Seleccionando el paquete xorg-sgml-doctools previamente no seleccionado.
Preparando para desempaquetar .../07-xorg-sgml-doctools_1%3a1.11-1.1_all.deb ...
Desempaquetando xorg-sgml-doctools (1:1.11-1.1) ...
Seleccionando el paquete x11proto-dev previamente no seleccionado.
Preparando para desempaquetar .../08-x11proto-dev_2021.5-1_all.deb ...
Desempaquetando x11proto-dev (2021.5-1) ...
Seleccionando el paquete libice-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../09-libice-dev_2%3a1.0.10-1build2_amd64.deb ...
Desempaquetando libice-dev:amd64 (2:1.0.10-1build2) ...
Seleccionando el paquete libpthread-stubs0-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../10-libpthread-stubs0-dev_0.4-1build2_amd64.deb ...
Desempaquetando libpthread-stubs0-dev:amd64 (0.4-1build2) ...
Seleccionando el paquete libsm-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../11-libsm-dev_2%3a1.2.3-1build2_amd64.deb ...
Desempaquetando libsm-dev:amd64 (2:1.2.3-1build2) ...
Seleccionando el paquete libxau-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../12-libxau-dev_1%3a1.0.9-1build5_amd64.deb ...
Desempaquetando libxau-dev:amd64 (1:1.0.9-1build5) ...
Seleccionando el paquete libxdmcp-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../13-libxdmcp-dev_1%3a1.1.3-0ubuntu5_amd64.deb ...
Desempaquetando libxdmcp-dev:amd64 (1:1.1.3-0ubuntu5) ...
Seleccionando el paquete xtrans-dev previamente no seleccionado.
Preparando para desempaquetar .../14-xtrans-dev_1.4.0-1_all.deb ...
Desempaquetando xtrans-dev (1.4.0-1) ...
Seleccionando el paquete libxcb1-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../15-libxcb1-dev_1.14-3ubuntu3_amd64.deb ...
Desempaquetando libxcb1-dev:amd64 (1.14-3ubuntu3) ...
Seleccionando el paquete libx11-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../16-libx11-dev_2%3a1.7.5-1ubuntu0.3_amd64.deb ...
Desempaquetando libx11-dev:amd64 (2:1.7.5-1ubuntu0.3) ...
Seleccionando el paquete libxt-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../17-libxt-dev_1%3a1.2.1-1_amd64.deb ...
Desempaquetando libxt-dev:amd64 (1:1.2.1-1) ...
Configurando libx11-xcb1:amd64 (2:1.7.5-1ubuntu0.3) ...
Configurando openjdk-11-jre-headless:amd64 (11.0.20.1+1-0ubuntu1~22.04) ...
Instalando una nueva versión del fichero de configuración /etc/java-11-openjdk/security/java.policy ...
Instalando una nueva versión del fichero de configuración /etc/java-11-openjdk/security/java.security ...
Configurando openjdk-11-jre:amd64 (11.0.20.1+1-0ubuntu1~22.04) ...
Configurando openjdk-11-jdk-headless:amd64 (11.0.20.1+1-0ubuntu1~22.04) ...
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jar para proveer /usr/bin/jar (jar) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jarsigner para proveer /usr/bin/jarsigner (jarsigner) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/javac para proveer /usr/bin/javac (javac) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/javadoc para proveer /usr/bin/javadoc (javadoc) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/javap para proveer /usr/bin/javap (javap) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jcmd para proveer /usr/bin/jcmd (jcmd) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jdb para proveer /usr/bin/jdb (jdb) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jdeprscan para proveer /usr/bin/jdeprscan (jdeprscan) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jdeps para proveer /usr/bin/jdeps (jdeps) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jfr para proveer /usr/bin/jfr (jfr) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jimage para proveer /usr/bin/jimage (jimage) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jinfo para proveer /usr/bin/jinfo (jinfo) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jlink para proveer /usr/bin/jlink (jlink) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jmap para proveer /usr/bin/jmap (jmap) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jmod para proveer /usr/bin/jmod (jmod) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jps para proveer /usr/bin/jps (jps) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jrunscript para proveer /usr/bin/jrunscript (jrunscript) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jshell para proveer /usr/bin/jshell (jshell) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jstack para proveer /usr/bin/jstack (jstack) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jstat para proveer /usr/bin/jstat (jstat) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jstatd para proveer /usr/bin/jstatd (jstatd) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/rmic para proveer /usr/bin/rmic (rmic) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/serialver para proveer /usr/bin/serialver (serialver) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jaotc para proveer /usr/bin/jaotc (jaotc) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jhsdb para proveer /usr/bin/jhsdb (jhsdb) en modo automático
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
Listamos versión que tenemos de Java.

```
melissa@melissa-linux:~$ java --version
openjdk 11.0.20.1 2023-08-24
OpenJDK Runtime Environment (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04)
OpenJDK 64-Bit Server VM (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04, mixed mode, sharing)

```

## ¿Cómo instalar una versión específica de Java? 
Para instalar Open JDK 11
```
melissa@melissa-linux:~$ sudo apt install openjdk-11-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
openjdk-11-jdk ya está en su versión más reciente (11.0.20.1+1-0ubuntu1~22.04).
fijado openjdk-11-jdk como instalado manualmente.
0 actualizados, 0 nuevos se instalarán, 0 para eliminar y 204 no actualizados.
```

Para instalar 13
```
melissa@melissa-linux:~$ sudo apt install openjdk-13-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
E: No se ha podido localizar el paquete openjdk-13-jdk
```

Para instalar 8 

```
melissa@melissa-linux:~$ sudo apt install openjdk-8-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
Se instalarán los siguientes paquetes adicionales:
  fonts-dejavu-extra libatk-wrapper-java libatk-wrapper-java-jni
  openjdk-8-jdk-headless openjdk-8-jre openjdk-8-jre-headless
Paquetes sugeridos:
  openjdk-8-demo openjdk-8-source visualvm fonts-nanum fonts-ipafont-gothic
  fonts-ipafont-mincho fonts-wqy-microhei fonts-wqy-zenhei
Se instalarán los siguientes paquetes NUEVOS:
  fonts-dejavu-extra libatk-wrapper-java libatk-wrapper-java-jni openjdk-8-jdk
  openjdk-8-jdk-headless openjdk-8-jre openjdk-8-jre-headless
0 actualizados, 7 nuevos se instalarán, 0 para eliminar y 204 no actualizados.
Se necesita descargar 45,8 MB de archivos.
Se utilizarán 156 MB de espacio de disco adicional después de esta operación.
¿Desea continuar? [S/n] s
Des:1 http://archive.ubuntu.com/ubuntu jammy/main amd64 fonts-dejavu-extra all 2.37-2build1 [2.041 kB]
Des:2 http://archive.ubuntu.com/ubuntu jammy/main amd64 libatk-wrapper-java all 0.38.0-5build1 [53,1 kB]
Des:3 http://archive.ubuntu.com/ubuntu jammy/main amd64 libatk-wrapper-java-jni amd64 0.38.0-5build1 [49,0 kB]
Des:4 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 openjdk-8-jre-headless amd64 8u382-ga-1~22.04.1 [30,8 MB]
Des:5 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 openjdk-8-jre amd64 8u382-ga-1~22.04.1 [75,4 kB]
Des:6 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 openjdk-8-jdk-headless amd64 8u382-ga-1~22.04.1 [8.851 kB]
Des:7 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 openjdk-8-jdk amd64 8u382-ga-1~22.04.1 [3.943 kB]
Descargados 45,8 MB en 5s (9.486 kB/s)
Seleccionando el paquete fonts-dejavu-extra previamente no seleccionado.
(Leyendo la base de datos ... 528457 ficheros o directorios instalados actualmen
te.)
Preparando para desempaquetar .../0-fonts-dejavu-extra_2.37-2build1_all.deb ...
Desempaquetando fonts-dejavu-extra (2.37-2build1) ...
Seleccionando el paquete libatk-wrapper-java previamente no seleccionado.
Preparando para desempaquetar .../1-libatk-wrapper-java_0.38.0-5build1_all.deb .
..
Desempaquetando libatk-wrapper-java (0.38.0-5build1) ...
Seleccionando el paquete libatk-wrapper-java-jni:amd64 previamente no selecciona
do.
Preparando para desempaquetar .../2-libatk-wrapper-java-jni_0.38.0-5build1_amd64
.deb ...
Desempaquetando libatk-wrapper-java-jni:amd64 (0.38.0-5build1) ...
Seleccionando el paquete openjdk-8-jre-headless:amd64 previamente no seleccionad
o.
Preparando para desempaquetar .../3-openjdk-8-jre-headless_8u382-ga-1~22.04.1_am
d64.deb ...
Desempaquetando openjdk-8-jre-headless:amd64 (8u382-ga-1~22.04.1) ...
Seleccionando el paquete openjdk-8-jre:amd64 previamente no seleccionado.
Preparando para desempaquetar .../4-openjdk-8-jre_8u382-ga-1~22.04.1_amd64.deb .
..
Desempaquetando openjdk-8-jre:amd64 (8u382-ga-1~22.04.1) ...
Seleccionando el paquete openjdk-8-jdk-headless:amd64 previamente no seleccionad
o.
Preparando para desempaquetar .../5-openjdk-8-jdk-headless_8u382-ga-1~22.04.1_am
d64.deb ...
Desempaquetando openjdk-8-jdk-headless:amd64 (8u382-ga-1~22.04.1) ...
Seleccionando el paquete openjdk-8-jdk:amd64 previamente no seleccionado.
Preparando para desempaquetar .../6-openjdk-8-jdk_8u382-ga-1~22.04.1_amd64.deb .
..
Desempaquetando openjdk-8-jdk:amd64 (8u382-ga-1~22.04.1) ...
Configurando openjdk-8-jre-headless:amd64 (8u382-ga-1~22.04.1) ...
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/orbd p
ara proveer /usr/bin/orbd (orbd) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/server
tool para proveer /usr/bin/servertool (servertool) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/tnames
erv para proveer /usr/bin/tnameserv (tnameserv) en modo automático
Configurando fonts-dejavu-extra (2.37-2build1) ...
Configurando libatk-wrapper-java (0.38.0-5build1) ...
Configurando libatk-wrapper-java-jni:amd64 (0.38.0-5build1) ...
Configurando openjdk-8-jdk-headless:amd64 (8u382-ga-1~22.04.1) ...
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/clhsdb par
a proveer /usr/bin/clhsdb (clhsdb) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/extcheck p
ara proveer /usr/bin/extcheck (extcheck) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/hsdb para 
proveer /usr/bin/hsdb (hsdb) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/idlj para 
proveer /usr/bin/idlj (idlj) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/javah para
 proveer /usr/bin/javah (javah) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/jhat para 
proveer /usr/bin/jhat (jhat) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/jsadebugd 
para proveer /usr/bin/jsadebugd (jsadebugd) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/native2asc
ii para proveer /usr/bin/native2ascii (native2ascii) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/schemagen 
para proveer /usr/bin/schemagen (schemagen) en modo automático
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

La version que se debe trabajar es la version 8. Para ello verificaremos la version de java que se esta ejecutando: 
```
melissa@melissa-linux:~$ java --version
openjdk 11.0.20.1 2023-08-24
OpenJDK Runtime Environment (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04)
OpenJDK 64-Bit Server VM (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04, mixed mode, sharing)

```

Como podemos observar tenemos la version 11, debemos configurar las variables de entorno para ponerla en la 8 que es con lo que vamos a trabajar.

## Configuracion de variables de entorno

El siguiente paso consiste en establecer las variables de entorno. Es necesario porque cuando se usa Java, Linux necesita saber dónde está ubicado el programa para ejecutarlo y qué versión de Java usar de forma predeterminada.

### LIstar las versiones de OpenJDK instaladas
```
melissa@melissa-linux:~$ sudo update-alternatives --config java
Existen 2 opciones para la alternativa java (que provee /usr/bin/java).

  Selección   Ruta                                            Prioridad  Estado
------------------------------------------------------------
* 0            /usr/lib/jvm/java-11-openjdk-amd64/bin/java      1111      modo automático
  1            /usr/lib/jvm/java-13-openjdk-amd64/bin/java      1111      modo manual
  2            /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java   1081      modo manual

Pulse <Intro> para mantener el valor por omisión [*] o pulse un número de selección: 2
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java para proveer /usr/bin/java (java) en modo manual
```

### Actualizacion de variables de entorno
Edita y modifica el fichero profile, con los comandos: 
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
