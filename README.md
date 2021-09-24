# Instalación JDK en Ubuntu
Cristian Cantelar Rodríguez

## Indice
1. [Introducción](#P1)
2. [Como instalar Java en Ubuntu desde repositorios](#P2)
3. [Comprobacion de version](#P3)

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
![image](img/paso1.png)
### Paso 2

Instalar la versión de java que quieras
```
sudo apt install openjdk-??-jdk
```
En este caso instalaremos la version de OpenJDK 8
```
sudo apt install openjdk-8-jdk
```
<div id='P3' />

### Paso 3

Verificar la version de JDK instalada
```
java 8version
```
En caso de querer verificar todas la versiones instaladas
```
ls /usr/lib/jvm
```
Con este simple proceso ya hemos instalado Java JDK en Ubuntu 20.04
