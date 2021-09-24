# Instalación JDK en Ubuntu
Cristian Cantelar Rodríguez

## Indice
1. [Introducción](#P1)
2. [Como instalar Java en Ubuntu desde repositorios](#P2)
3. [Comprobacion de version](#P3)
4. [Configuración de las variables de entorno](#P4)

<div id='P1' />

## Introduccíon
Java Development Kit o JDK es un software que provee herramientas de desarrollo para la creacion de programas en java.
Es ideal para crear y desarrollar aplicaciones o sitios webs.

<div id='P2' />

## Como instalar Java en Ubuntu desde repositorios

### Paso 1

Accedamos a la terminal y lo primero que haremos es actualizar el sistema con el comando:
```
sudo apt-get update
```
![image](/Paso1.PNG)
  
### Paso 2

Instalar la versión de java que quieras
```
sudo apt install openjdk-??-jdk
```
En este caso instalaremos la version de OpenJDK 8
```
sudo apt install openjdk-8-jdk
```
![image](/Paso2.PNG)

<div id='P3' />

### Paso 3

Verificar la version de JDK instalada
```
java -version
```
![image](/Paso3.PNG)

Si no se ejecuta la versión 8 deberas hacer lo siguiente


<div id='P4' />

### Configuración de las variables de entorno
Este paso es necesario ya que al usar Java, Linux no sabe dónde esta ubicado el programa.
Para solucionar eso tendremos que:

#### Listar la versiones de OpenJDK instaladas
```
ls /usr/lib/jvm
```
#### Actualización de las variables de entorno
Edita y modifica el fichero profile
```
nano /etc/profile
```
Realiza los siguiente cambios en la versión 8
```
# Java version
JAVA_HOME=/usr/lib/jvm/_____openJdk_____
PATH=$PATH:$HOME/bin:$JAVA_HOME/bin
export JAVA_HOME
export JRE_HOME
export PATH
```
![image](/Paso4.PNG)

Con este simple proceso ya hemos instalado Java JDK en Ubuntu 20.04
