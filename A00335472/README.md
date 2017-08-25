### Taller 1
**Universidad ICESI**  
**Curso:** Sistemas Operativos  
**Docente:** Daniel Barragán C.  
**Tema:** Comandos de Linux, Estructura de directorio, Virtualización  
**Correo:** daniel.barragan at correo.icesi.edu.co


### Objetivos
* Conocer y emplear comandos de Linux para la realización de tareas administrativas

### Prerrequisitos
* Virtualbox o WMWare
* Máquina virtual con sistema operativo CentOS7

### Descripción
El primer taller del curso sistemas operativos trata sobre el sistema operativo Linux, la estructura de sus directorios y virtualización 

### Actividades

1. Explique la función de los directorios en la raíz de sistema operativo Linux-CentOS.
Proporcione ejemplos de los archivos que se encuentran en cada directorio (explique al menos un
archivo por directorio).

| Directorio | Función |
|------|------|
| bin | Almacenar todos los binarios necesarios para garantizar las funciones básicas del usuario. Permitir ejecución de de utilidades estándar de la terminal de Linux. |
| boot | Almacenar todos los ejecutables y archivos que son necesarios en el proceso de arranque del sistema antes que el kernel inice en el sistema. |
| dev | Incluir dispositivos de almacenamiento conectados al sistema en forma de archivos. |
| etc | Almacenar archivos de configuración de los componentes del SO, programas y aplicaciones. |
| home | Almacenar todos los archivos de los usuarios y archivos temporales de aplicaciones de usuario. |
| lib | Incluir las bibliotecas para que se puedan ejecutar todos los binarios y módulos del kernel. |
| media | Punto de montaje de todos los volúmenes lógicos, como USB, otras particiones de disco, etc. |
| mnt | Cumple funciones similares a media, no se suele utilizar y es un directorio vacío. |
| opt | Almacenar archivos de solo lectura que son parte de programas auto-contenidos. | 
| proc | Contener información de los procesos y aplicaciones que se están ejecutando en el sistema. No guarda nada y el directorio está vacío. |
| root | Directorio del usuario root. |
| sbin | Almacenar todos los binarios necesarios para garantizar las funciones básicas del  SO. |
| srv | Almacenar archivos y directorios relativos a servidores instalados. |
| sys | Contener archivos virtuales con informacion sobre el kernel relativa eventos del SO. |
| tmp | Almacenar archivos temporales de todo tipo. |
| usr | Almacenar todos los archivos de lectura relativos a las utilidades del usuario. |
| var | Contener varios archivos con información del sistema, como archivos de logs, emails, bases de datos, información almacenada en la caché, información relativa a los paquetes de aplicaciones almacenados en /opt, etc. |

| Directorio   | Archivo ejemplo | Descripción del contenido del directorio  |
|------|------|------|
| bin | zsoelim | Lee archivos y reemplaza lineas de tipo .so |
| boot | grub | Crea la lista de SO's para arrancar en el menu de interfaz de GRUB |
| dev| zero | Cada vez que se lee de este device se retorna 0 |
| etc | hostname | Contiene el hostname de la máquina |
| home | operativos | Carpeta con los archivos del usuario operativos  |
| lib | kbd | Contiene keymaps | 
| media | cdrom | Punto montaje unidad de cd | 
| mnt | cdrom | Punto montaje unidad de cd en mnt. |
| opt | /opt/someapp/bin/foo | Archivo de configuración de un programa auto-contenido | 
| proc | cmdline | Línea de comandos del Kernel |
| root | anaconda-ks.cfg | Archivo de Kickstart provisto por RedHat para instalar el SO |
| sbin | zdump | Muestra información horaria especificada | 
| srv | www | Directorio de servidor web instalado |
| sys | class | Agrupar los dispositivos que son similares de manera virtual | 
| tmp | yum.log | Información sobre instalaciones de yum | 
| usr | /usr/src/kernels | Archivo source del kernel | 
| var | games | Todo tipo de datos variable relacionados a juego en /usr |







2. En una tabla como se muestra a continuación escriba 10 comandos de Linux no visto en clase. Puede incluir comandos que funcionan una vez han sido instalados con yum

| Comando   | Usuario | Descripción   |
|------|------|------|
| # zdump <zone>| root | Muestra información horaria especificada |
| # zsoelim | root | Lee archivos y reemplaza lineas de tipo .so |
| # reboot | root | Renicia el sistema |
| # id <user> | operativos | Muestra UID, GID, GROUPS del usuario user. |
| # ping <host> | operativos | Permite conocer si host esta activo en la red |
| # ifconfig eth0 up : down | root | Permite activar o bajar la tarjeta de red eth0 del sistema |
| # yum check-update | root | Permite determinar si hay actualizaciones disponibles |
| # yum search <keyword> | root | Buscar paquetes que contengan el keyword dado en todos los repositorios |
| # ls -lh  | operativos | Permite listar los archivos de forma paginada |
| # wc <file> | operativos | Permite mostrar el número de palabras, líneas y caracteres de un archivo. |

3. ¿Cuál es la utilidad del comando printenv en Linux?, Investigue acerca de la creación de variables de ambiente en Linux y como hacerlas permanentes. Cree una variable de ambiente, hágala permanente y muestre evidencias del funcionamiento.

## PRINTENV

Muestra el valor de todas las variables de ambiente; si se indica un nombre de variable, muestra el valor de esa variable.

## VARIABLE AMBIENTE PERMANENTE

* https://docs.google.com/document/d/10v85Hb0jjBQYTfqPZP_WySyD2mTkJexdHs3Qe0RSClU/edit?usp=sharing

### Nota

El informe debe ser entregado en formato README.md y debe ser subido a un repositorio de github. El repositorio de github debe ser un fork de https://github.com/ICESI-Training/so-workshop1 y para la entrega deberá hacer un Pull Request (PR) respetando la estructura definida. El código fuente y la url de github deben incluirse en el informe.  

## Referencias

* https://computernewage.com/2015/06/14/el-arbol-de-directorios-de-linux-al-detalle-que-contiene-cada-carpeta/
* http://www.tldp.org/LDP/Linux-Filesystem-Hierarchy/html/
* https://github.com/ICESI/so-commands/tree/master/centos7
* https://cmdchallenge.com  
* https://www.gutenberg.org
* http://www.sysadmit.com/2016/04/linux-variables-de-entorno-permanentes.html
