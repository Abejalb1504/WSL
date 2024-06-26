# 2.- Instalación de WSL
## 2.1.- Prerrequisitos

Antes de instalar WSL en un sistema Windows, es importante verificar que se cumplan los siguientes prerrequisitos:

- **Para Windows**:
  - El sistema operativo Windows debe estar actualizado a la versión Windows 10 1607 (Anniversary Update) o posterior.
  - Se requiere un procesador de 64 bits con soporte para virtualización de hardware.
  - Disponer de suficiente espacio en disco para instalar las distribuciones de Linux que desees utilizar.

- **Para Windows Server**:
  - El sistema operativo Windows Server con al menos la versión 1809 (Windows Server 2019 LTSC) o posterior.
  - Se necesita un procesador de 64 bits con soporte para virtualización de hardware.
  - Disponer de suficiente espacio en disco para instalar las distribuciones de Linux que desees utilizar.

Es importante tener en cuenta que esta guía de instalación utilizará Windows 11 como ejemplo.

## 2.2.- Instalación WLS + Ubuntu
El comando de instalación de **WLS** por defecto añade una maquina ubuntu por lo que se realizará la guia de ambas instalaciones de manera conjunta.
1. **Ejecutamos la terminal de PowerShell como administrador.**
---
   ![Captura2](/Imagenes/Captura1.png)

---
2. **En el terminal ejecutamos el comando "wsl --install" y relanzamos el terminal**
---
Este comando habilitará las características necesarias para ejecutar WSL e instalará la distribución Ubuntu de Linux.

   ![Captura1](/Imagenes/Captura2.png)

---
3. **Crear un usuario y contraseña en el nuevo ubuntu**
---


   ![Captura1](/Imagenes/Captura3.png)

   ---
Con esto tendremos todo lo necesario para poder usar Ubuntu dentro de Windows.

## 2.3.- Instalación Otra maquina 
En caso de querer utilizar otro sistema operativo en lugar de Ubuntu, Microsoft ofrece muchas opciones para elegir. En este tutorial, se mostrará cómo instalar Debian, pero es posible ver todas las opciones disponibles utilizando el siguiente comando:

```powershell
wsl --list --online
```
1. **Ejecutamos la terminal de PowerShell como administrador.**
---
   ![Captura2](/Imagenes/Captura1.png)

---

2. **Esta vez el comando cambia**
---
Para poder especificar que distribucion de linux de las posibles tendremos que usar:
```powershell
wsl --install -d Debian
```

   ![Captura1](/Imagenes/Captura4.png)

---

3. **Dependiendo de la distribucion te peidra crear un usuario en el mismo terminal**
---
En este caso no hemos tenido que abrir powershell de nuevo y ha pedido nuevo usuario y contraseña, no solo eso, tambien ha entrado directamente a Debian.


   ![Captura1](/Imagenes/Captura5.png)

---

[Volver](/README.md)
