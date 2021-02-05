# Práctica 1 - Configuración del entorno de trabajo y herramientas

En esta práctica llevaremos a cabo la configuración de la máquina virtual que tienen disponible a través
del servicio IaaS de la ULL, además de la instalación y configuración de todas las herramientas necesarias
para comenzar a trabajar en la asignatura.

Dado que tendrán que llevar a cabo un informe acerca de todos los pasos que han seguido, además de enumerar
los diferentes problemas a los que se han enfrentado con sus respectivas soluciones, les aconsejo que lean
esta breve [introducción a Markdown](https://guides.github.com/features/mastering-markdown/). De este modo,
podrán utilizar dicho lenguaje para escribir el informe en el repositorio de Github asociado a la asignación
de Github Classroom que tendrán que aceptar.

## Algunas tareas previas

1. Cumplimente la [encuesta de elección de grupo de trabajo](https://campusingenieriaytecnologia.ull.es/mod/choicegroup/view.php?id=281122).
2. Cumplimente la [encuesta sobre expectativas y conocimientos previos](https://campusingenieriaytecnologia.ull.es/mod/feedback/view.php?id=281123).
3. Dese de alta en el aula [Google Classroom](https://campusingenieriaytecnologia.ull.es/mod/assign/view.php?id=281124) de la asignatura.
4. Acepte la [asignación de Github Classroom](https://classroom.github.com/a/ckIr4G7P) asociada a esta práctica.

## Configuración de la máquina virtual en el IaaS

Lo primero que debemos hacer es configurar el servicio VPN de la ULL en el caso de que estemos tratando de utilizar el servicio IaaS desde
fuera de la red universitaria. Para ello, debemos acceder a la
[documentación de configuración de la VPN de la ULL](https://www.ull.es/servicios/stic/2020/12/01/servicio-de-vpn-de-la-ull/)
y descargar las instrucciones correspondientes a nuestro sistema operativo. Siga dichas instrucciones y trate de conectarse a la VPN de la ULL.

Una vez conectado a la VPN, deberá acceder al [Servicio IaaS de la ULL](https://iaas.ull.es/) e introducir sus credenciales ULL. A continuación, se le mostrará un panel de control con las diferentes máquinas virtuales que tiene asociadas a su cuenta. Si no lo ha hecho antes,
deberá iniciar la máquina virtual que se llama *DSI*. Al arrancar dicha máquina, se le asignará una máquina virtual del pool de máquinas virtuales
de la asignatura. Sabrá que lo anterior ha sucedido debido a que su máquina pasará a tener un número como sufijo, por ejemplo *DSI-76*.

Haga clic en el nombre de su máquina virtual y, en la parte derecha de la interfaz, donde se indica *Interfaces de red*, podrá conocer
la IP asignada a la interfaz de su máquina. Conociendo dicha IP, ya podrá conectarse por SSH a su máquina. Es importante recordar que
siempre tiene que estar conectado a la VPN de la ULL para trabajar con una máquina virtual del IaaS. Para conectarse por SSH a su
máquina virtual, abra una terminal y teclee lo siguiente:

```bash
ssh usuario@10.6.XXX.XXX
```

Introduzca *yes* y pulse intro ante la pregunta:

```bash
The authenticity of host \'10.6.XXX.XXX (10.6.XXX.XXX)\' can\'t be established.
ECDSA key fingerprint is SHA256:1Xm4M66FeBUSiykP7SqJgObwjmVs2gEouBhy1PTWDV4.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```

La contraseña que debe introducir ahora es *usuario* (las credenciales por defecto son *usuario*, *usuario* para el nombre de usuario y
contraseña, respectivamente). Una vez introducida dicha contraseña, el propio sistema le indicará que la modifique. Para ello, deberá
introducir su contraseña actual (*usuario*) y, luego, su nueva contraseña por duplicado. Trate de recordar su nueva contraseña
o apúntela en un lugar seguro. Una vez hecho lo anterior, tendrá que volver a iniciar una conexión SSH con su máquina, pero esta vez
deberá usar su nueva contraseña para acceder.



## Instalación de software en la máquina virtual del IaaS

## Instalación de Visual Studio Code