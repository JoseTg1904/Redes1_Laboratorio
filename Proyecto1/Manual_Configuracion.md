<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [Proyecto 1](#proyecto-1)
      - [Grupo 1](#grupo-1)
      - [Guatemala 31 de Agosto 2021](#guatemala-31-de-agosto-2021)
- [Tabla de Contenido](#tabla-de-contenido)
- [**1. Configuración inicial topologia 1**](#1-configuraci%C3%B3n-inicial-topologia-1)
  - [**1.1 Configuración ESW1**](#11-configuraci%C3%B3n-esw1)
    - [1.1.1 Configuración de puertos modo truncal](#111-configuraci%C3%B3n-de-puertos-modo-truncal)
    - [1.1.2 Configuración de protocolo vtp](#112-configuraci%C3%B3n-de-protocolo-vtp)
    - [1.1.2 demostracion de protocolo vtp](#112-demostracion-de-protocolo-vtp)
  - [**1.2 Configuración ESW2**](#12-configuraci%C3%B3n-esw2)
    - [1.2.1 Configuración de puertos modo truncal](#121-configuraci%C3%B3n-de-puertos-modo-truncal)
    - [1.2.2 Configuración de puertos modo acceso](#122-configuraci%C3%B3n-de-puertos-modo-acceso)
    - [1.2.3 Configuración de protocolo vtp](#123-configuraci%C3%B3n-de-protocolo-vtp)
    - [1.2.4 Desmostración de protocolo vtp](#124-desmostraci%C3%B3n-de-protocolo-vtp)
  - [**1.3 Configuración ESW3**](#13-configuraci%C3%B3n-esw3)
    - [1.3.1 Configuración de puertos modo truncal](#131-configuraci%C3%B3n-de-puertos-modo-truncal)
    - [1.3.2 Configuración de puertos modo acceso](#132-configuraci%C3%B3n-de-puertos-modo-acceso)
    - [1.3.3 Configuración de protocolo vtp](#133-configuraci%C3%B3n-de-protocolo-vtp)
    - [1.3.3 Demostración de protocolo vtp](#133-demostraci%C3%B3n-de-protocolo-vtp)
  - [**1.4 Configuración nube**](#14-configuraci%C3%B3n-nube)
  - [**1.5 Configuración ip de VPCS**](#15-configuraci%C3%B3n-ip-de-vpcs)
    - [1.5.1 Configuración Conta_1 y Conta_2](#151-configuraci%C3%B3n-conta_1-y-conta_2)
    - [1.5.2 Configuración Informatica_1](#152-configuraci%C3%B3n-informatica_1)
    - [1.5.3 Configuración RRHH_1 y RRHH_2](#153-configuraci%C3%B3n-rrhh_1-y-rrhh_2)
    - [1.5.4 Configuración Ventas_1](#154-configuraci%C3%B3n-ventas_1)
- [**2. Configuración inicial topologia 2**](#2-configuraci%C3%B3n-inicial-topologia-2)
  - [**2.1 Configuración ESW4**](#21-configuraci%C3%B3n-esw4)
    - [2.1.1 Crear vlans](#211-crear-vlans)
    - [2.1.2 Ver vlans](#212-ver-vlans)
    - [2.1.3 Crar modos truncales parte 1](#213-crar-modos-truncales-parte-1)
    - [2.1.4 Crar modos truncales parte2](#214-crar-modos-truncales-parte2)
    - [2.1.5 Ver modos truncales](#215-ver-modos-truncales)
    - [2.1.6 Vtp server](#216-vtp-server)
    - [2.1.7 Vtp status](#217-vtp-status)
    - [2.1.8 Vtp version 2](#218-vtp-version-2)
    - [2.1.9 Vtp pruning](#219-vtp-pruning)
    - [2.1.10 Habilitar STP](#2110-habilitar-stp)
    - [2.1.11 Configuraciones STP](#2111-configuraciones-stp)
    - [2.1.12 STP puertos block](#2112-stp-puertos-block)
  - [**2.2 Configuración ESW7**](#22-configuraci%C3%B3n-esw7)
    - [2.2.1 Configuracion modo truncal p1](#221-configuracion-modo-truncal-p1)
    - [2.2.2 Configuracion modo truncal p2](#222-configuracion-modo-truncal-p2)
    - [2.2.3 Configuracion modo truncal p3](#223-configuracion-modo-truncal-p3)
    - [2.2.4 Configuracion modo acceso](#224-configuracion-modo-acceso)
    - [2.2.5 Configuración cliente VTP](#225-configuraci%C3%B3n-cliente-vtp)
    - [2.2.6 Ver puertos TR](#226-ver-puertos-tr)
    - [2.2.7 Ver vlans](#227-ver-vlans)
    - [2.2.8 VTP status](#228-vtp-status)
  - [**2.3 Configuración ESW6**](#23-configuraci%C3%B3n-esw6)
    - [2.3.1 Configuración de puertos modo truncal parte 1](#231-configuraci%C3%B3n-de-puertos-modo-truncal-parte-1)
    - [2.3.2 Configuración de puertos modo truncal parte 2](#232-configuraci%C3%B3n-de-puertos-modo-truncal-parte-2)
    - [2.3.3 Configuración de puertos modo truncal parte 3](#233-configuraci%C3%B3n-de-puertos-modo-truncal-parte-3)
    - [2.3.4 Configuración de puertos modo truncal parte 4](#234-configuraci%C3%B3n-de-puertos-modo-truncal-parte-4)
    - [2.3.5 Configuración cliente VTP](#235-configuraci%C3%B3n-cliente-vtp)
    - [2.3.6 Configuración puertos TR](#236-configuraci%C3%B3n-puertos-tr)
    - [2.3.7 Configuración vlans](#237-configuraci%C3%B3n-vlans)
    - [2.3.8 Vlan status](#238-vlan-status)
  - [**2.4 Configuración ESW5**](#24-configuraci%C3%B3n-esw5)
    - [2.4.1 Configuración modo truncal p1](#241-configuraci%C3%B3n-modo-truncal-p1)
    - [2.4.2 Configuración modo truncal p2](#242-configuraci%C3%B3n-modo-truncal-p2)
    - [2.4.3 Configuración cliente VTP](#243-configuraci%C3%B3n-cliente-vtp)
    - [2.4.4 Puertos troncales](#244-puertos-troncales)
    - [2.4.5 Vlans de clientes](#245-vlans-de-clientes)
    - [2.4.6 VTP status](#246-vtp-status)
  - [**2.5 Configuración ip de Informatica_2**](#25-configuraci%C3%B3n-ip-de-informatica_2)
- [**3. Configuración inicial topologia 3**](#3-configuraci%C3%B3n-inicial-topologia-3)
  - [**3.1 Configuración de los switches**](#31-configuraci%C3%B3n-de-los-switches)
    - [3.1.1 Switch S1](#311-switch-s1)
    - [3.1.2 Switch S2](#312-switch-s2)
    - [3.1.3 Switch S3](#313-switch-s3)
    - [3.1.4 Switch S4](#314-switch-s4)
  - [**3.2 Configuración de los switches en modo acceso**](#32-configuraci%C3%B3n-de-los-switches-en-modo-acceso)
    - [3.2.1 Switch S1](#321-switch-s1)
    - [3.2.2 Switch S2](#322-switch-s2)
    - [3.2.3 Switch S3](#323-switch-s3)
    - [3.2.4 Switch S4](#324-switch-s4)
  - [**3.3 Configuración de los switches en modo truncal**](#33-configuraci%C3%B3n-de-los-switches-en-modo-truncal)
    - [3.3.1 Switch S1](#331-switch-s1)
    - [3.3.2 Switch S2](#332-switch-s2)
    - [3.3.3 Switch S3](#333-switch-s3)
    - [3.3.4 Switch S4](#334-switch-s4)
  - [**3.4 Configuración de vtp en los switch**](#34-configuraci%C3%B3n-de-vtp-en-los-switch)
    - [3.4.1 Switch S1](#341-switch-s1)
    - [3.4.2 Switch S2](#342-switch-s2)
    - [3.4.3 Switch S3](#343-switch-s3)
    - [3.4.4 Switch S4](#344-switch-s4)
  - [**3.5 Configuración de las VPCS(SERVERS)**](#35-configuraci%C3%B3n-de-las-vpcsservers)
    - [3.5.1 Servidor contabilidad](#351-servidor-contabilidad)
    - [3.5.2 Servidor Informatica](#352-servidor-informatica)
    - [3.5.3 Servidor RRHH](#353-servidor-rrhh)
    - [3.5.4 Servidor Ventas](#354-servidor-ventas)
- [**4. Pings topologia 1**](#4-pings-topologia-1)
  - [**4.1 Ping entre conta_1 y conta_2**](#41-ping-entre-conta_1-y-conta_2)
  - [**4.2 Ping entre conta_1 y server**](#42-ping-entre-conta_1-y-server)
  - [**4.3 Ping entre conta_2 y conta_1**](#43-ping-entre-conta_2-y-conta_1)
  - [**4.4 Ping entre conta_2 y server**](#44-ping-entre-conta_2-y-server)
  - [**4.5 Ping entre vlans**](#45-ping-entre-vlans)
  - [**4.6 Ping entre informatica_1 e informatica_2**](#46-ping-entre-informatica_1-e-informatica_2)
  - [**4.7 Ping entre informatica_1 y server**](#47-ping-entre-informatica_1-y-server)
  - [**4.8 Ping entre RRHH_1 y RRHH_2**](#48-ping-entre-rrhh_1-y-rrhh_2)
  - [**4.9 Ping entre RRHH_1 y server**](#49-ping-entre-rrhh_1-y-server)
  - [**4.10 Ping entre RRHH_2 y RRHH_1**](#410-ping-entre-rrhh_2-y-rrhh_1)
  - [**4.11 Ping entre RRHH_2 y Server**](#411-ping-entre-rrhh_2-y-server)
  - [**4.12 Ping entre ventas_1 y Server**](#412-ping-entre-ventas_1-y-server)
- [**5. Pings topologia 2**](#5-pings-topologia-2)
  - [**5.1 Ping entre informatica_1 e informatica_2**](#51-ping-entre-informatica_1-e-informatica_2)
  - [**5.2 Ping**](#52-ping)
  - [**5.3 No ping**](#53-no-ping)
- [**6. Pings topologia 3**](#6-pings-topologia-3)
  - [**6.1 Ping conta**](#61-ping-conta)
  - [**6.2 Ping informatica**](#62-ping-informatica)
  - [**6.3 Ping rrhh**](#63-ping-rrhh)
  - [**6.4 Ping ventas**](#64-ping-ventas)
  - [**6.5 Ping conta diferente departamento**](#65-ping-conta-diferente-departamento)
  - [**6.6 Ping informatica diferente departamento**](#66-ping-informatica-diferente-departamento)
  - [**6.7 Ping rrhh diferente departamento**](#67-ping-rrhh-diferente-departamento)
  - [**6.8 Ping ventas diferente departamento**](#68-ping-ventas-diferente-departamento)
- [**7. Requerimientos de equipo**](#7-requerimientos-de-equipo)
- [**8. Requerimientos para ejecutar archivos gns3**](#8-requerimientos-para-ejecutar-archivos-gns3)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


<p style="font-size: 18px">
Universidad de San Carlos de Guatemala
<br>
Facultad de Ingeniería
<br>
Escuela de Ciencias y Sistemas
<br>
Redes de Computadoras 1
<br>
Ing. Miguel Marin de León
<br>
Aux. Juan Pablo García Monzón
</p>

<br><br><br><br>



<h1 align="center" style="font-size: 40px; font-weight: bold;">Proyecto 1</h1>

<br><br><br>

<h4 align="center" style="font-size: 30px; font-weight: bold;">Grupo 1</h4>

<br><br>


<div align="center">

| Carnet | Nombre |
| :-: | :-:| 
| 201700965 | José Carlos I Alonzo Colocho |
| 201700319 | Estanley Rafael Cóbar García |
| 201709140 | Oscar Armin Crisostomo Ruiz |
| 201709309 | José Alejandro Santizo Cotto  |

</div>

<br><br>

<h4 align="center" style="font-size: 18px; font-weight: bold;">Guatemala 31 de Agosto 2021</h4>


*** 


<br><br><br><br>

*** 

<h1>Tabla de Contenido</h1>



- [Proyecto 1](#proyecto-1)
      - [Grupo 1](#grupo-1)
      - [Guatemala 31 de Agosto 2021](#guatemala-31-de-agosto-2021)
- [Tabla de Contenido](#tabla-de-contenido)
- [**1. Configuración inicial topologia 1**](#1-configuraci%C3%B3n-inicial-topologia-1)
  - [**1.1 Configuración ESW1**](#11-configuraci%C3%B3n-esw1)
    - [1.1.1 Configuración de puertos modo truncal](#111-configuraci%C3%B3n-de-puertos-modo-truncal)
    - [1.1.2 Configuración de protocolo vtp](#112-configuraci%C3%B3n-de-protocolo-vtp)
    - [1.1.2 demostracion de protocolo vtp](#112-demostracion-de-protocolo-vtp)
  - [**1.2 Configuración ESW2**](#12-configuraci%C3%B3n-esw2)
    - [1.2.1 Configuración de puertos modo truncal](#121-configuraci%C3%B3n-de-puertos-modo-truncal)
    - [1.2.2 Configuración de puertos modo acceso](#122-configuraci%C3%B3n-de-puertos-modo-acceso)
    - [1.2.3 Configuración de protocolo vtp](#123-configuraci%C3%B3n-de-protocolo-vtp)
    - [1.2.4 Desmostración de protocolo vtp](#124-desmostraci%C3%B3n-de-protocolo-vtp)
  - [**1.3 Configuración ESW3**](#13-configuraci%C3%B3n-esw3)
    - [1.3.1 Configuración de puertos modo truncal](#131-configuraci%C3%B3n-de-puertos-modo-truncal)
    - [1.3.2 Configuración de puertos modo acceso](#132-configuraci%C3%B3n-de-puertos-modo-acceso)
    - [1.3.3 Configuración de protocolo vtp](#133-configuraci%C3%B3n-de-protocolo-vtp)
    - [1.3.3 Demostración de protocolo vtp](#133-demostraci%C3%B3n-de-protocolo-vtp)
  - [**1.4 Configuración nube**](#14-configuraci%C3%B3n-nube)
  - [**1.5 Configuración ip de VPCS**](#15-configuraci%C3%B3n-ip-de-vpcs)
    - [1.5.1 Configuración Conta_1 y Conta_2](#151-configuraci%C3%B3n-conta_1-y-conta_2)
    - [1.5.2 Configuración Informatica_1](#152-configuraci%C3%B3n-informatica_1)
    - [1.5.3 Configuración RRHH_1 y RRHH_2](#153-configuraci%C3%B3n-rrhh_1-y-rrhh_2)
    - [1.5.4 Configuración Ventas_1](#154-configuraci%C3%B3n-ventas_1)
- [**2. Configuración inicial topologia 2**](#2-configuraci%C3%B3n-inicial-topologia-2)
  - [**2.1 Configuración ESW4**](#21-configuraci%C3%B3n-esw4)
    - [2.1.1 Crear vlans](#211-crear-vlans)
    - [2.1.2 Ver vlans](#212-ver-vlans)
    - [2.1.3 Crar modos truncales parte 1](#213-crar-modos-truncales-parte-1)
    - [2.1.4 Crar modos truncales parte2](#214-crar-modos-truncales-parte2)
    - [2.1.5 Ver modos truncales](#215-ver-modos-truncales)
    - [2.1.6 Vtp server](#216-vtp-server)
    - [2.1.7 Vtp status](#217-vtp-status)
    - [2.1.8 Vtp version 2](#218-vtp-version-2)
    - [2.1.9 Vtp pruning](#219-vtp-pruning)
    - [2.1.10 Habilitar STP](#2110-habilitar-stp)
    - [2.1.11 Configuraciones STP](#2111-configuraciones-stp)
    - [2.1.12 STP puertos block](#2112-stp-puertos-block)
  - [**2.2 Configuración ESW7**](#22-configuraci%C3%B3n-esw7)
    - [2.2.1 Configuracion modo truncal p1](#221-configuracion-modo-truncal-p1)
    - [2.2.2 Configuracion modo truncal p2](#222-configuracion-modo-truncal-p2)
    - [2.2.3 Configuracion modo truncal p3](#223-configuracion-modo-truncal-p3)
    - [2.2.4 Configuracion modo acceso](#224-configuracion-modo-acceso)
    - [2.2.5 Configuración cliente VTP](#225-configuraci%C3%B3n-cliente-vtp)
    - [2.2.6 Ver puertos TR](#226-ver-puertos-tr)
    - [2.2.7 Ver vlans](#227-ver-vlans)
    - [2.2.8 VTP status](#228-vtp-status)
  - [**2.3 Configuración ESW6**](#23-configuraci%C3%B3n-esw6)
    - [2.3.1 Configuración de puertos modo truncal parte 1](#231-configuraci%C3%B3n-de-puertos-modo-truncal-parte-1)
    - [2.3.2 Configuración de puertos modo truncal parte 2](#232-configuraci%C3%B3n-de-puertos-modo-truncal-parte-2)
    - [2.3.3 Configuración de puertos modo truncal parte 3](#233-configuraci%C3%B3n-de-puertos-modo-truncal-parte-3)
    - [2.3.4 Configuración de puertos modo truncal parte 4](#234-configuraci%C3%B3n-de-puertos-modo-truncal-parte-4)
    - [2.3.5 Configuración cliente VTP](#235-configuraci%C3%B3n-cliente-vtp)
    - [2.3.6 Configuración puertos TR](#236-configuraci%C3%B3n-puertos-tr)
    - [2.3.7 Configuración vlans](#237-configuraci%C3%B3n-vlans)
    - [2.3.8 Vlan status](#238-vlan-status)
  - [**2.4 Configuración ESW5**](#24-configuraci%C3%B3n-esw5)
    - [2.4.1 Configuración modo truncal p1](#241-configuraci%C3%B3n-modo-truncal-p1)
    - [2.4.2 Configuración modo truncal p2](#242-configuraci%C3%B3n-modo-truncal-p2)
    - [2.4.3 Configuración cliente VTP](#243-configuraci%C3%B3n-cliente-vtp)
    - [2.4.4 Puertos troncales](#244-puertos-troncales)
    - [2.4.5 Vlans de clientes](#245-vlans-de-clientes)
    - [2.4.6 VTP status](#246-vtp-status)
  - [**2.5 Configuración ip de Informatica_2**](#25-configuraci%C3%B3n-ip-de-informatica_2)
- [**3. Configuración inicial topologia 3**](#3-configuraci%C3%B3n-inicial-topologia-3)
  - [**3.1 Configuración de los switches**](#31-configuraci%C3%B3n-de-los-switches)
    - [3.1.1 Switch S1](#311-switch-s1)
    - [3.1.2 Switch S2](#312-switch-s2)
    - [3.1.3 Switch S3](#313-switch-s3)
    - [3.1.4 Switch S4](#314-switch-s4)
  - [**3.2 Configuración de los switches en modo acceso**](#32-configuraci%C3%B3n-de-los-switches-en-modo-acceso)
    - [3.2.1 Switch S1](#321-switch-s1)
    - [3.2.2 Switch S2](#322-switch-s2)
    - [3.2.3 Switch S3](#323-switch-s3)
    - [3.2.4 Switch S4](#324-switch-s4)
  - [**3.3 Configuración de los switches en modo truncal**](#33-configuraci%C3%B3n-de-los-switches-en-modo-truncal)
    - [3.3.1 Switch S1](#331-switch-s1)
    - [3.3.2 Switch S2](#332-switch-s2)
    - [3.3.3 Switch S3](#333-switch-s3)
    - [3.3.4 Switch S4](#334-switch-s4)
  - [**3.4 Configuración de vtp en los switch**](#34-configuraci%C3%B3n-de-vtp-en-los-switch)
    - [3.4.1 Switch S1](#341-switch-s1)
    - [3.4.2 Switch S2](#342-switch-s2)
    - [3.4.3 Switch S3](#343-switch-s3)
    - [3.4.4 Switch S4](#344-switch-s4)
  - [**3.5 Configuración de las VPCS(SERVERS)**](#35-configuraci%C3%B3n-de-las-vpcsservers)
    - [3.5.1 Servidor contabilidad](#351-servidor-contabilidad)
    - [3.5.2 Servidor Informatica](#352-servidor-informatica)
    - [3.5.3 Servidor RRHH](#353-servidor-rrhh)
    - [3.5.4 Servidor Ventas](#354-servidor-ventas)
- [**4. Pings topologia 1**](#4-pings-topologia-1)
  - [**4.1 Ping entre conta_1 y conta_2**](#41-ping-entre-conta_1-y-conta_2)
  - [**4.2 Ping entre conta_1 y server**](#42-ping-entre-conta_1-y-server)
  - [**4.3 Ping entre conta_2 y conta_1**](#43-ping-entre-conta_2-y-conta_1)
  - [**4.4 Ping entre conta_2 y server**](#44-ping-entre-conta_2-y-server)
  - [**4.5 Ping entre vlans**](#45-ping-entre-vlans)
  - [**4.6 Ping entre informatica_1 e informatica_2**](#46-ping-entre-informatica_1-e-informatica_2)
  - [**4.7 Ping entre informatica_1 y server**](#47-ping-entre-informatica_1-y-server)
  - [**4.8 Ping entre RRHH_1 y RRHH_2**](#48-ping-entre-rrhh_1-y-rrhh_2)
  - [**4.9 Ping entre RRHH_1 y server**](#49-ping-entre-rrhh_1-y-server)
  - [**4.10 Ping entre RRHH_2 y RRHH_1**](#410-ping-entre-rrhh_2-y-rrhh_1)
  - [**4.11 Ping entre RRHH_2 y Server**](#411-ping-entre-rrhh_2-y-server)
  - [**4.12 Ping entre ventas_1 y Server**](#412-ping-entre-ventas_1-y-server)
- [**5. Pings topologia 2**](#5-pings-topologia-2)
  - [**5.1 Ping entre informatica_1 e informatica_2**](#51-ping-entre-informatica_1-e-informatica_2)
  - [**5.2 Ping**](#52-ping)
  - [**5.3 No ping**](#53-no-ping)
- [**6. Pings topologia 3**](#6-pings-topologia-3)
  - [**6.1 Ping conta**](#61-ping-conta)
  - [**6.2 Ping informatica**](#62-ping-informatica)
  - [**6.3 Ping rrhh**](#63-ping-rrhh)
  - [**6.4 Ping ventas**](#64-ping-ventas)
  - [**6.5 Ping conta diferente departamento**](#65-ping-conta-diferente-departamento)
  - [**6.6 Ping informatica diferente departamento**](#66-ping-informatica-diferente-departamento)
  - [**6.7 Ping rrhh diferente departamento**](#67-ping-rrhh-diferente-departamento)
  - [**6.8 Ping ventas diferente departamento**](#68-ping-ventas-diferente-departamento)
- [**7. Requerimientos de equipo**](#7-requerimientos-de-equipo)
- [**8. Requerimientos para ejecutar archivos gns3**](#8-requerimientos-para-ejecutar-archivos-gns3)




<br><br><br><br>


# **1. Configuración inicial topologia 1**

<br>

<div align="center">

![Imagen 1.1 Descarga de VirtualBox](./imagenes/topologia1/topologia.jpg)

</div>

***
## **1.1 Configuración ESW1**
***
### 1.1.1 Configuración de puertos modo truncal

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw1_truncal1.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw1_truncal2.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw1_truncal3.png)

</div>

***
### 1.1.2 Configuración de protocolo vtp

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw1_vtp.png)

</div>

***
### 1.1.2 demostracion de protocolo vtp

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw1_vtp_demostracion.png)

</div>

***
## **1.2 Configuración ESW2**
***
### 1.2.1 Configuración de puertos modo truncal

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw2_truncal1.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw2_truncal2.png)

</div>

***
### 1.2.2 Configuración de puertos modo acceso

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw2_acceso1.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw2_acceso2.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw2_acceso3.png)

</div>

***

***
### 1.2.3 Configuración de protocolo vtp

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw2_vtp.png)

</div>

***

### 1.2.4 Desmostración de protocolo vtp

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw2_vtp_demostracion.png)

</div>

***

## **1.3 Configuración ESW3**

***
### 1.3.1 Configuración de puertos modo truncal

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw3_truncal1.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw3_truncal2.png)

</div>

***

### 1.3.2 Configuración de puertos modo acceso

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw3_acceso1.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw3_acceso2.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw3_acceso3.png)

</div>

***

### 1.3.3 Configuración de protocolo vtp

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw3_vtp.png)

</div>

***

### 1.3.3 Demostración de protocolo vtp

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/esw3_vtp_demostracion.png)

</div>

***

## **1.4 Configuración nube**

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/nube.png)

</div>

***

## **1.5 Configuración ip de VPCS**

***
### 1.5.1 Configuración Conta_1 y Conta_2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/conta1_ip.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/conta2_ip.png)

</div>

***

### 1.5.2 Configuración Informatica_1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/informatica1_ip.png)

</div>

***

### 1.5.3 Configuración RRHH_1 y RRHH_2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/rrhh1_ip.png)

</div>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/rrhh2_ip.png)

</div>

***

### 1.5.4 Configuración Ventas_1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/configuracion/ventas1_ip.png)

</div>

***



















# **2. Configuración inicial topologia 2**

<br>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/topologia.jpg)

</div>

***
## **2.1 Configuración ESW4**
***
### 2.1.1 Crear vlans

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/1.ESW4_SERVER_crearVlans.png)

</div>

***
### 2.1.2 Ver vlans

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/2.ESW4_SERVER_verVLANS.png)

</div>

***
### 2.1.3 Crar modos truncales parte 1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/3.ESW4_SERVER_crearmodostruncales_p1.png)

</div>

***

### 2.1.4 Crar modos truncales parte2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/4.ESW4_SERVER_crearmodostruncales_p2.png)

</div>

***

### 2.1.5 Ver modos truncales

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/5.ESW4_SERVER_ver_modos_truncales.png)

</div>

***

### 2.1.6 Vtp server

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/6.ESW4_SERVER_vtp_server.png)

</div>

***

### 2.1.7 Vtp status

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/7.ESW4_SERVER_vtp_status.png)

</div>

***

### 2.1.8 Vtp version 2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/8.ESW4_SERVER_vtp_version2.png)

</div>

***

### 2.1.9 Vtp pruning

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/9.ESW4_SERVER_vtp_pruning.png)

</div>

***

### 2.1.10 Habilitar STP

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/10.ESW4_SERVER_stp_habilitar.png)

</div>

***

### 2.1.11 Configuraciones STP

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/11.ESW4_SERVER_stp_configuraciones.png)

</div>

***

### 2.1.12 STP puertos block

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/12.ESW4_SERVER_stp_puertos_block.png)

</div>

***

## **2.2 Configuración ESW7**
***
### 2.2.1 Configuracion modo truncal p1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/13.ESW7_CLIENT_modo_trunk_p1.png)

</div>

***
### 2.2.2 Configuracion modo truncal p2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/14.ESW7_CLIENT_modo_trunk_p2.png)

</div>

***

### 2.2.3 Configuracion modo truncal p3

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/14.ESW7_CLIENT_modo_trunk_p3.png)

</div>

***

### 2.2.4 Configuracion modo acceso

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/15.ESW7_CLIENT_modo_access.png)

</div>

***

### 2.2.5 Configuración cliente VTP

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/16.ESW7_CLIENT_vtp_client.png)

</div>

***

### 2.2.6 Ver puertos TR

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/17.ESW7_CLIENT_ver_puertos-tr.png)

</div>

***

### 2.2.7 Ver vlans

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/18.ESW7_CLIENT_ver_vlans.png)

</div>

***

### 2.2.8 VTP status

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/19.ESW7_CLIENT_vtp_status.png)

</div>

***







## **2.3 Configuración ESW6**

***
### 2.3.1 Configuración de puertos modo truncal parte 1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/20.ESW6_CLIENT_modo_truncal_p1.png)

</div>

***

### 2.3.2 Configuración de puertos modo truncal parte 2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/21.ESW6_CLIENT_modo_truncal_p2.png)

</div>

***

### 2.3.3 Configuración de puertos modo truncal parte 3

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/22.ESW6_CLIENT_modo_truncal_p3.png)

</div>

***

### 2.3.4 Configuración de puertos modo truncal parte 4

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/23.ESW6_CLIENT_modo_truncal_p4.png)

</div>

***

### 2.3.5 Configuración cliente VTP

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/24.ESW6_CLIENT_vtp_client.png)

</div>

***

### 2.3.6 Configuración puertos TR

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/25.ESW6_CLIENT_puertos_tr.png)

</div>

### 2.3.7 Configuración vlans

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/26.ESW6_CLIENT_vlans.png)

</div>

### 2.3.8 Vlan status

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/27.ESW6_CLIENT_vtp_status.png)

</div>










## **2.4 Configuración ESW5**

***

### 2.4.1 Configuración modo truncal p1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/28.ESW5_CLIENT_modo_truncal_p1.png)

</div>

***

### 2.4.2 Configuración modo truncal p2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/29.ESW5_CLIENT_modo_truncal_p2.png)

</div>

***

### 2.4.3 Configuración cliente VTP

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/30.ESW5_CLIENT_vtp_client.png)

</div>

***

### 2.4.4 Puertos troncales

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/31.ESW5_CLIENT_puertos_trunk.png)

</div>

***

### 2.4.5 Vlans de clientes

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/32.ESW5_CLIENT_vlans_client.png)

</div>

***

### 2.4.6 VTP status

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/33.ESW5_CLIENT_vtp_status.png)

</div>

***




## **2.5 Configuración ip de Informatica_2**

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/configuracion/34.informatica_2_configuracion.png)

</div>

***










# **3. Configuración inicial topologia 3**

<br>

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/topologia.jpg)

</div>

***
## **3.1 Configuración de los switches**
***
### 3.1.1 Switch S1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/configuracion/s1.png)

</div>

***

### 3.1.2 Switch S2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/configuracion/s2.png)

</div>

***

### 3.1.3 Switch S3

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/configuracion/s3.png)

</div>

***

### 3.1.4 Switch S4

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/configuracion/s4.png)

</div>

***




## **3.2 Configuración de los switches en modo acceso**
***
### 3.2.1 Switch S1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/modo_acceso/s1_modo_accesso_conta.png)

</div>

***

### 3.2.2 Switch S2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/modo_acceso/s2_modo_accesso_RRHH.png)

</div>

***

### 3.2.3 Switch S3

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/modo_acceso/s3_modo_accesso_informatica.png)

</div>

***

### 3.2.4 Switch S4

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/modo_acceso/s4_modo_accesso_ventas.png)

</div>

***





## **3.3 Configuración de los switches en modo truncal**
***
### 3.3.1 Switch S1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/modo_truncal/s1.png)

</div>

***

### 3.3.2 Switch S2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/modo_truncal/s2.png)

</div>

***

### 3.3.3 Switch S3

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/modo_truncal/s3.png)

</div>

***

### 3.3.4 Switch S4

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/modo_truncal/s4.png)

</div>

***





## **3.4 Configuración de vtp en los switch**
***
### 3.4.1 Switch S1

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/vtp/s1.png)

</div>

***

### 3.4.2 Switch S2

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/vtp/s2.png)

</div>

***

### 3.4.3 Switch S3

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/vtp/s3.png)

</div>

***

### 3.4.4 Switch S4

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/vtp/s4.png)

</div>

***







## **3.5 Configuración de las VPCS(SERVERS)**
***
### 3.5.1 Servidor contabilidad

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/servers/server_conta.png)

</div>

***

### 3.5.2 Servidor Informatica

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/servers/server_informatica.png)

</div>

***

### 3.5.3 Servidor RRHH

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/servers/server_rrhh.png)

</div>

***

### 3.5.4 Servidor Ventas

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/configuracion/servers/server_ventas.png)

</div>

***







# **4. Pings topologia 1**

<br>

## **4.1 Ping entre conta_1 y conta_2**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_conta1_conta2.png)

</div>

***

## **4.2 Ping entre conta_1 y server**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_conta1_server.png)

</div>

***

## **4.3 Ping entre conta_2 y conta_1**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_conta2_conta1.png)

</div>

***

## **4.4 Ping entre conta_2 y server**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_conta2_server.png)

</div>

***

## **4.5 Ping entre vlans**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_entre_vlans.png)

</div>

***

## **4.6 Ping entre informatica_1 e informatica_2**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_informatica1_informatica2.png)

</div>

***

## **4.7 Ping entre informatica_1 y server**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_informatica1_server.png)

</div>

***


## **4.8 Ping entre RRHH_1 y RRHH_2**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_rrhh1_rrhh2.png)

</div>

***

## **4.9 Ping entre RRHH_1 y server**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_rrhh1_server.png)

</div>

***

## **4.10 Ping entre RRHH_2 y RRHH_1**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_rrhh2_rrhh1.png)

</div>

***

## **4.11 Ping entre RRHH_2 y Server**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_rrhh2_server.png)

</div>

***

## **4.12 Ping entre ventas_1 y Server**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia1/pings/ping_ventas1_server.png)

</div>

***














# **5. Pings topologia 2**

<br>

## **5.1 Ping entre informatica_1 e informatica_2**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/pings/35.informatica_2_ping_informatica1.png)

</div>

***

## **5.2 Ping**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/pings/35.informatica_2_ping.png)

</div>

***

## **5.3 No ping**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia2/pings/37.informatica_2_no_ping.png)

</div>

***











# **6. Pings topologia 3**

<br>

## **6.1 Ping conta**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/pings/conta.png)

</div>

***

## **6.2 Ping informatica**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/pings/informatica.png)

</div>

***

## **6.3 Ping rrhh**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/pings/rrhh.png)

</div>

***

## **6.4 Ping ventas**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/pings/ventas.png)

</div>

***

## **6.5 Ping conta diferente departamento**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/nopings/conta.png)

</div>

***

## **6.6 Ping informatica diferente departamento**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/nopings/informatica.png)

</div>

***

## **6.7 Ping rrhh diferente departamento**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/nopings/rrhh.png)

</div>

***

## **6.8 Ping ventas diferente departamento**


<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./imagenes/topologia3/nopings/venta.png)

</div>

***

# **7. Requerimientos de equipo**

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./requerimientosEquipo.png)

</div>

# **8. Requerimientos para ejecutar archivos gns3**

<div align="center">

![Imagen 1.1. Descarga de VirtualBox](./reqgns3.jpg)

</div>