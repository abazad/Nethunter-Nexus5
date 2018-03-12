<img src="https://github.com/robriap/my-compute-experiments-learning/blob/master/nethunter-nexus-5/files/IMG_20180302_144459.jpg">


##      EL PROCESO QUE YO HE SEGUIDO
  Manuales de instalacion hay muchos, lo que voy a incluir en esta carpeta es simplemente
  el que yo he seguido y las modificaciones de instalacion o reinstalaciones que he hecho
  con el fin de crearlos en "new branchs" para llevar un control o que quien quiera pueda 
  crear nuevos branch añadiendo o modificando cosas.
  
###     EL manual que he seguido esta en los archivos de esta carpeta.
     https://github.com/robriap/my-compute-experiments-learning/blob/master/nethunter-nexus-5/Instalacion/Nexus%205_%20Desbloquear%20bootloader%20-%20Recovery%20TWRP%20-%20Root.pdf
     

###     EL adb que instala lo que pone en el manual es este
     https://github.com/robriap/my-compute-experiments-learning/blob/master/nethunter-nexus-5/Instalacion/adb-setup-1.4.3.exe
     
     El archivo original es de xda donde explican más detalladamente el asunto.
     https://forum.xda-developers.com/showthread.php?t=2588979
     
    
# ______

Desbloquear el bootloader del Nexus 5 implica que todo el contenido del equipo sera eliminado, respalda tus apps y archivos antes de realizar esto.

## 1.  Encender el Nexus 5 en modo fastboot presionando Power + Vol-, conectar el cable USB a la PC. 
## 2.  Abrir  una  ventana  de  comandos  en  nuestra  carpeta  de  trabajo  (C:\adb) presionando  shift  +  clic  derecho  o  utilizar  el  comando  cd  para  indicar  la  ruta de la carpeta donde se encuentra instalado fastboot. 
## 3.  Escribir el comando fastboot oem unlock 
## 4.  Aparecerá  una  advertencia,  con  las  teclas  de  volumen  resalta  la  opción YES y selecciónala con el botón de power.
## 5.  Al terminar colocamos el comando presionamos enter para así reiniciar el equipo. Este reinicio tomara unos minutos pues android debe volver a construir el cache.

## Nota: Si tienes problemas asegurate de que la computadora ve al Nexus 5, usa el comando fastboot devices para ver si el Nexus 5 aparece listado.

#      Instalar TWRP en el Nexus 5 

Este es el twrp que he instalado yo: 
https://github.com/robriap/my-compute-experiments-learning/blob/master/nethunter-nexus-5/Instalacion/twrp-3.2.1-1-hammerhead.img

El  TWRP  es  la  herramienta  que  nos  permitirá  flashear  zips  en  el  Nexus  5  y muchas cosas mas. Antes  de  comenzar  debemos  colocar  el  arhivo  .img  del  TWRP  en  nuestra carpeta de trabajo  C:\adb 
## 1.  Encender el Nexus 5 en modo fastboot presionando Power + Vol-, conectar el cable USB a la PC. 
## 2.  Abrir  una  ventana  de  comandos  en  nuestra  carpeta  de  trabajo  (C:\adb) presionando  shift  +  clic  derecho  o  utilizar  el  comando  cd  para  indicar  la  ruta de la carpeta donde se encuentra instalado fastboot. 
## 3.  Escribir el comando
Donde XXX es el nombre completo del archivo del TWRP. 
Por ejemplo: 
### fastboot flash recovery  twrp-3.2.1-1-hammerhead.img

## 4.  Al  terminar  puedes  reiniciar  el  Nexus  5  utilizando  fastboot  reboot  o ingresar  directamente  en  el  menú  recovery,  para  ello  utiliza  las  teclas  de volumen hasta que veas Recovery Mode y luego presiona power. 

#       Rootear Nexus 5 con ROM Stock 6.0.1 

Este es el root que he instalado yo
https://github.com/robriap/my-compute-experiments-learning/blob/master/nethunter-nexus-5/Instalacion/SR5-SuperSU-v2.82-SR5-20171001224502.zip

El  acceso  root  o  acceso  administrativo  es  un  clásico  y  algo  necesario  para aquellos  que  queremos  tener  control  total  sobre  nuestros  teléfonos.  Como  en este  caso  hablamos  de  una  rom  stock,  es  decir,  el  firmware  oficial,  el  root  es muy  importante  para  modificar  el  sistema  a  nuestro  gusto,  en  especial  si deseamos usar  Xposed Framework  y sus módulos. Luego  de  descargar  el  ZIP  de  SuperSU  copíalo  a  la  memoria  del  Nexus  5  y reinicialo en modo recovery. 
## 1.  Una  vez  en  TWRP,  entra  en  Install  y  busca  el  archivo  zip  del  instalador  de SuperSU, desliza el control para instalarlo. 
## 2.  Cuando  termine  selecciona  Wipe  Dalvik/Cache  y  desliza  el  el  control  para realizar esta operación 
## 3.  Finalmente  selecciona  reboot  system  para  reiniciar  el  Nexus  5.  Android deberá  construir  nuevamente  el  cache  por  lo  que  debes  ser  paciente,  este inicio tomara unos minutos.
## 4.  Al  culminar  habrás  rooteado  tu  Nexus  5  y  tendrás  la  aplicación  de  SuperSu disponible en el launcher. 

# ______________________

# La instalacion de Nethunter
## Primero leí bien la información de esta página
https://www.offensive-security.com/kali-linux-nethunter-download/
## Y la de esta
https://github.com/offensive-security/kali-nethunter/wiki

## Descargue el archivo de nethunter correspondiente en mi caso Nexus 5 con 6.0.1
De todos modos seguramente con el tiempo se actualizará de la página oficial así 
que por si necesito el archivo que he instalado en la primera vez ... Lo puse aqui:
https://drive.google.com/a/slhsscience.net/file/d/1XJmX_wDKpAEtGCDtuNoQjPC0qWNcX6fg/view?usp=drivesdk

## Lo he metido en la sd y después he iniciado con el recovery e instalado el archivo seleccionando todas las opciones que te plantea el instalador (Excepto la de root puesto que ya está instalado)

## Al terminar el proceso reinicio y arranco la aplicación nethunter que preparará el sistema. 
## Lo vuelvo a cerrar y ya está lista la instalación propiamente dicha.


       
