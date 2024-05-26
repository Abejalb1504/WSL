# 1.- Introducción a Windows Subsystem Linux
![wsl](/Imagenes/wsl.jpg)
## 1.1.- ¿Que es WSL?
WSL (Windows Subsystem for Linux) es una característica de Windows 10 y Windows Server 2019 que permite a los usuarios ejecutar un entorno GNU/Linux directamente en Windows, sin la sobrecarga de una máquina virtual tradicional o de arranque dual. WSL proporciona una capa de compatibilidad para ejecutar binarios de Linux nativos en Windows.

### Características Principales
* Compatibilidad con distribuciones de Linux: WSL permite instalar y ejecutar distribuciones populares de Linux como Ubuntu, Debian, OpenSUSE, Kali Linux, entre otras, directamente desde la Microsoft Store.
* Integración con el sistema de archivos de Windows: Permite acceder a los archivos de Windows desde el entorno de Linux y viceversa. Las rutas del sistema de archivos de Windows pueden ser montadas en /mnt dentro de WSL.
* Bajo consumo de recursos: A diferencia de las máquinas virtuales, WSL utiliza una cantidad mínima de recursos del sistema, ya que no necesita emular hardware completo.
* Desempeño nativo: Ejecuta aplicaciones de Linux con un rendimiento casi nativo al del sistema operativo Linux.
* Soporte de herramientas de desarrollo: Permite el uso de herramientas y scripts de desarrollo de Linux, como bash, ssh, git, y muchas otras, directamente en Windows.
### Versiones de WSL
WSL tiene dos versiones principales, cada una con sus propias características y ventajas:

* WSL 1: La primera versión de WSL, que traduce las llamadas del kernel de Linux en llamadas al kernel de Windows. Es ligera y rápida, pero tiene algunas limitaciones de compatibilidad y rendimiento con ciertas aplicaciones de Linux que dependen de características del kernel no implementadas en esta versión.

* WSL 2: Introducida en 2019, esta versión incluye un kernel de Linux completo y real que se ejecuta en una máquina virtual ligera, utilizando tecnología de virtualización de Hyper-V. WSL 2 ofrece una mejor compatibilidad y rendimiento que WSL 1, permitiendo una ejecución más eficiente de aplicaciones y herramientas de Linux.

Actualmente se recomienda el uso de WSL 2 debido a su mejor compatibilidad, mayor rendimiento, y soporte mejorado para contenedores como Docker.


## 1.2.- Pros y contras.
### Beneficios de usar WSL
* Facilita el desarrollo multiplataforma: Los desarrolladores pueden escribir scripts y aplicaciones en un entorno Linux y probarlos directamente en Windows.
* Integración con el entorno de desarrollo de Windows: Permite usar editores y herramientas de desarrollo de Windows (como Visual Studio Code) junto con herramientas y scripts de Linux.
* Mejor soporte para contenedores y microservicios: Facilita el uso de herramientas como Docker en un entorno Windows para desarrollar y ejecutar contenedores basados en Linux.
* Sin necesidad de arranque dual: Los usuarios pueden ejecutar aplicaciones de Linux junto con aplicaciones de Windows, sin necesidad de reiniciar el sistema.

### Desventajas y riesgos de WSL
* Compatibilidad limitada: Algunas aplicaciones y servicios de Linux pueden no funcionar correctamente o no estar completamente soportados.
* Seguridad: Es importante destacar que al implementar WSL en tu dispositivo, este queda expuesto a las vulnerabilidades inherentes a Linux,
  lo que puede aumentar la carga administrativa y los riesgos de brechas de seguridad.
* Rendimiento variable: Aunque WSL 2 ofrece un buen rendimiento, ciertas cargas de trabajo intensivas pueden no funcionar tan eficientemente como en un entorno Linux nativo.
* Dependencia de Windows: WSL depende de la estabilidad y el rendimiento del sistema operativo Windows, lo que puede ser una limitación en entornos críticos.
* Consumo de recursos: WSL 2, al utilizar una máquina virtual ligera, consume más recursos del sistema que WSL 1, lo que puede ser un problema en dispositivos con hardware limitado.


## 1.3.- Cuando usarlo y cuando no
WSL es una herramienta versátil que ofrece numerosos beneficios para los desarrolladores y usuarios que desean trabajar en un entorno Linux dentro de Windows.
Es especialmente útil para aquellos que buscan desarrollar y probar aplicaciones en múltiples plataformas, ya que proporciona una forma conveniente de ejecutar herramientas y scripts de Linux sin la necesidad de cambiar de sistema operativo. 
Además, es ideal para quienes desean aprender y familiarizarse con Linux, ya que ofrece un entorno seguro y controlado para experimentar con comandos y prácticas de línea de comandos.

Por otro lado, aunque WSL ofrece muchas ventajas, no es la mejor opción para todas las situaciones. No se recomienda para aplicaciones críticas en producción que requieren un alto nivel de estabilidad y seguridad, ya que las vulnerabilidades inherentes a Linux pueden exponer el sistema a riesgos adicionales. 
Tampoco es adecuado para procesos que demandan un rendimiento intensivo, ya que el rendimiento de WSL puede no ser óptimo en comparación con un entorno Linux nativo. 
Además, en entornos con altos requisitos de seguridad o necesidades de compatibilidad total con hardware, es preferible optar por soluciones que ofrezcan un mayor control y aislamiento.

[Volver](/README.md)

