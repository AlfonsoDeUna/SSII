# Clase fecha: 11_01

## INTRODUCCIÓN A VIRTUAL BOX

Necesitamos instalar VirtualBox. https://www.virtualbox.org/
Ubuntu 20.04. https://releases.ubuntu.com/20.04/

## introducción (personal)

## PRÁCTICA 1: CREACIÓN MÁQUINAS VIRTUALES INFRAESTRUCTURA WEB o LAMP ( INSTALACIÓN Y GESTIÓN DE MÁQUINAS VIRTUALES)

Un cliente nos ha pedido que montemos un Wordpress en un servidor propio, para ello debemos montar una *infraestructura web dinámica*. Para ello debemos instalar un Apache Web Server y una base de datos como MySQL. Pero antes debemos montar una máquina virtual en VirtualBox (IMAGINAMOS QUE ESTAMOS EN EL SERVIDOR DEL CLIENTE AUNQUE SEA NUESTRA PROPIA MÁQUINA). 

REQUISITOS HARDWARE: (VAMOS VIENDO EN CLASE LAS CARACTERÍSTICAS DE PARAMETRIZACIÓN DE UNA MÁQUINA)

  * 2GB DE RAM
  * 10 GB disco SATA
  * 2 CPUs virtuales
  * iso UBUNTU 20.04 LINUX ( profesor )
  * RED EN MODO NAT
 
INSTALACIÓN DE UBUNTU: (
  * PARTICIÓN / SWAP (ESTÁNDAR)
  
NOMBRE MÁQUINA: login DAM / Password: 2020  
  
INSTALACIÓN PASOS:

  *instalación de Apache 2. Servidor Web
   
   ```
   $ sudo apt update
   $ sudo apt install apache2
   
   ```
  
  *configuración del firewall.
  
  
  
 Las guías de DigitalOcean son bastante buenas aunque puede que no funcionen porque no están actualizadas.
 
 https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-20-04-es
 
* LINKS INTERESANTES PARA LA INSTALACIÓN * 
https://www.muylinux.com/2018/06/18/guia-instalacion-ubuntu-18-04-lts/


## MODIFICACIONES SOBRE LA PRÁCTICA 1 (AMPLIACIÓN)

### CREAR UN CLON DE LA MÁQUINA A MODO DE BACKUP

### CREAR UNA EXPORTACIÓN E IMPORTANCIÓN EN FORMATO .OVA
  * PARA PROBARLO SÚBELO A DRIVE Y COMPÁRTELO CON TU COMPAÑERO, TIENES QUE PODER IMPORTAR CON LA HERRAMIENTA DE VIRTUALBOX

### [SITUACIÓN PRÁCTICA REAL] [SPR] NOS HEMOS QUEDADO SIN DISCO DURO: !!!!!! PELIGRO!!!! EL CLIENTE LLAMA ENFADADO, QUÉ HEMOS HECHO MAL.

Esta situación es muy típica en entornos en los que las máquinas están en constante actualización de datos y en uso. ¿Qué pasa si nos quedamos sin disco duro? ¿Cómo lo podemos arreglar?

  #### OPCIONES: 
  #### MONTAR UN 2º DISCO DURO / DARLE FORMATO
  
  #### AMPLIAR EL DISCO DURO PRINCIPAL VÍA VIRTUALBOX
  
  
  # LIBROS Y DOCUMENTACIÓN DE VIRTUALBOX
  
  * VirtualBox 3.1: Beginner's Guide (Inglés) : https://www.amazon.es/Virtualbox-3-1-Alfonso-V-Romero/dp/1847199143/ref=sr_1_7?__mk_es_ES=%C3%85M%C3%85%C5%BD%C3%95%C3%91&dchild=1&keywords=virtualbox+libro&qid=1609150256&sr=8-7
  
  
