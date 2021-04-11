<hr />
<img width="150px" height="150px" style="border-radius: 50%;"  src="https://utp.ac.pa/documentos/2015/imagen/logo_utp_1_300.png"/>

<center>
	<em></em>Universidad Tecnológica de Panamá<br />
	<em></em>Facultad de Ingeniería de Sistemas Computacionales<br />
	<em></em>Ingeniería en sistemas computacionales<br />
	<em>Tema: </em>ArchLinux<br />
	<em>Profesora: </em>Yarisol Castillo <br />
	<em>Autores: </em>Hewel Ochoa, Vaihinger Vega<br />
	<em>Año: </em>2021<br />
	<em>Creado: </em>31/03/2021<br />
</center>
<hr />

# ArchLinux

* Es una de las mas completas y complejas distribuciones de Linux
* Se compone en su mayor parte de software libre y de código abierto
* Apoya la participación comunitaria
* Su modelo de desarrollo es de tipo [Liberación continua](https://es.wikipedia.org/wiki/Liberaci%C3%B3n_continua)
* Su enfoque de diseño se basa en el [Principio KISS](https://es.wikipedia.org/wiki/Principio_KISS)

## Arquitecturas
* [x86-64](https://es.wikipedia.org/wiki/X86-64 "X86-64")
* [ARM](https://es.wikipedia.org/wiki/Arquitectura_ARM "Arquitectura ARM")
* [I686](https://es.wikipedia.org/wiki/I686 "I686") 

## Versión
**Arch Linux** no tiene un planeamiento de lanzamientos, sino son simplemente «capturas» del conjunto de paquetes actual del repositorios compatibles con la totalidad del sistema. Su desarrollo se basa en un _modelo_ llamado Liberación continua (del inglés "Rolling Release"). Este enfoque de desarrollo, similar a la distribución avanzada Gentoo Linux, promueve mayores prestaciones en cuanto al uso de las últimas versiones más nuevas de software.

Como herramienta para administrarlo, Arch Linux se apoya en su gestor de paquetes, llamado Pacman. Este programa, escrito en lenguaje C y de uso exclusivo por invocación desde línea de comandos desde una consola de terminal, se obtienen las últimas versiones posibles de programas de forma sencilla..

**Pacman** no solo se utiliza para instalar, eliminar y actualizar paquetes. Incluso es capaz de obtener las últimas versiones de software crítico como imágenes del kernel, y de esa manera brindar soporte con las últimas novedades del hardware.

### ISO
-   **ISO Size:** 750.3 MB
-   **Included Kernel:** 5.11.11
- **Current Release:** 2021.04.01
-   [Guía de Instalación](https://wiki.archlinux.org/index.php/Installation_guide)

## Usuarios a los que esta destinado y su utilidad principal
- Orientada a usuarios avanzados.
- Desarrolladores
- Seguridad informática
- Usuarios con pocos recursos

## Características
A diferencia de las distribuciones populares basadas en el Núcleo Linux como Ubuntu o Linux Mint, **Arch Linux** no posee herramientas de configuración automática, compartiendo así la misma filosofía de distribuciones, como Slackware. Para instalar y configurar este sistema operativose necesita un grado de conocimiento superior al básico. No obstante, se puede mantener y administrar el sistema de forma sencilla. Los creadores y la comunidad, denominan como "filosofía", los siguientes tres aspectos:

-   Mantener el sistema lo más simple y ligero posible, siguiendo el llamado principio KISS.
-   Los principios del continuador del liderazgo del proyecto, Aaron Griffin, también son tomados como referencia: _«Fiarse de las GUIs para construir y configurar tu sistema operativo termina dañando a los usuarios finales. Intentar ocultar la complejidad del sistema, termina complicando al sistema. Las capas de abstracción que sirven para ocultar el funcionamiento interno nunca son una cosa buena. En cambio, los componentes internos deberían de ser diseñados de forma que no necesiten ser ocultados»_.
-   Arch Linux permite al usuario hacer las contribuciones que desee, mientras estas no vayan en contra de la filosofía.

El enfoque de diseño del equipo de desarrollo, sigue el principio KISS ("Keep It Simple Stupid" o "Mantenlo Simple Estúpido"). Según los creadores y la Comunidad, el principio se centra en elegancia, exactitud, minimalismo y simplicidad. **Arch Linux** define simplicidad como _«...una estructura base compacta sin añadidos innecesarios, modificaciones, o complicaciones, que permite a un usuario individual modificar el sistema de acuerdo a sus propias necesidades»_. La simplicidad de su estructura no implica sencillez en su manejo.

## Requerimientos de Hardware
-   Ordenador de 32 bits o 64 bits.
-   530 MB de RAM cómo mínimo
    -   Si instalas un entorno gráfico (escritorio), necesitarás más memoria RAM según el que hayas escogido.
    -   Se recomienda al menos 1GB – 2GB de RAM para entornos gráficos.
-   2 GB de espacio en disco como mínimo
    -   Igual que la memoria RAM requerida, según la cantidad de paquetes que vayas a instalar, necesitarás más.
    -   Se recomiendo tener unos 10GB – 20GB si utilizas un entorno gráfica, así como si pretendes instalar varios programas/paquetes.
-   Conexión a Internet para descargar los paquetes necesarios (sea WIFI o Ethernet)

## Enlace de descarga
Qué la descarga se basa en mirror list (listas de espejo), es mejor escoger una cercana a tu país.

En nuestro caso solamente podemos usar colombia u estados unidos:
https://archlinux.org/download/

# Virtualización de ArchLinux
Decídimos usar hyper-v, ya que lo incluye windows 10.

## Qué es Hyper-v?
- Hyper-V es una tecnología de **Microsoft** que permite a los usuarios crear entornos de servidores virtuales.
- Ejecutar y administrar múltiples sistemas operativos en un solo servidor físico.
- En otras palabras **crear y administrar máquinas virtuales**.

## Qué permite hyper-v?
-   Crear y eliminar máquinas virtuales.
-   Monitorea el tiempo de actividad, la utilización del ancho de banda, el consumo de CPU y RAM.
-   Realice copias de seguridad.
-   Asignar recursos.
-   Tener la herramienta de administración correcta es clave para su éxito con la virtualización.

## Instalar Hyper-v
Para instalar y usar el rol Hyper-V, se necesita lo siguiente:

-  Un procesador basado en x64. Hyper-V está disponible en las versiones basadas en x64 de Windows Server 2008, concretamente, las versiones basadas en x64 de Windows Server 2008 Standard, Windows Server 2008 Enterprise y Windows Server 2008 Datacenter.  
      
-  Virtualización asistida por hardware. Está disponible en procesadores que incluyen una opción de virtualización; concretamente, Intel Virtualization Technology (Intel VT) o AMD Virtualization (AMD-V).  
      
-  La Prevención de ejecución de datos (DEP) implementada por hardware debe estar disponible y habilitada. Concretamente, debe habilitar el bit XD de Intel (bit ejecutar deshabilitado) o el bit NX de AMD (bit no ejecutar).

## Activar hyper-v
Para activar hyper-v en Windows debemos:
1.  Abra una consola de PowerShell como administrador.
2.  Ejecute el siguiente comando:
```PowerShell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper\-V -All
```

Si no se pudo encontrar el comando, asegúrese de que está ejecutando PowerShell como administrador.

Cuando la instalación se haya completado, reinicie.
### Habilite Hyper-V con CMD y DISM
La herramienta de administración y mantenimiento de imágenes de implementación (DISM) ayuda a configurar Windows y las imágenes. 
- Entre sus muchas aplicaciones, DISM puede habilitar funciones de Windows mientras el sistema operativo está en ejecución.

Para habilitar el rol de Hyper-V usando DISM:
1.  Abra una sesión de PowerShell o CMD como administrador.
2.  Escriba el siguiente comando:
```PowerShell
DISM /Online /Enable-Feature /All /FeatureName:Microsoft-Hyper\-V
```

## Crear un conmutador virtual
1.  Haga clic con el botón derecho en Windows PowerShell y seleccione **Ejecutar como administrador**.
2.  Busque los adaptadores de red existentes mediante la ejecución del cmdlet [Get-NetAdapter](https://docs.microsoft.com/es-es/powershell/module/netadapter/get-netadapter) . Anote el nombre del adaptador de red que desea usar para el conmutador virtual.
3.  Cree un conmutador virtual con el cmdlet [New-VMSwitch](https://docs.microsoft.com/es-es/powershell/module/hyper-v/new-vmswitch) . Por ejemplo, para crear un conmutador virtual externo denominado ExternalSwitch, con el adaptador de red Ethernet y con **permitir que el sistema operativo de administración comparta este adaptador de red** activado, ejecute el siguiente comando.
```PowerShell
New-VMSwitch -name ExternalSwitch \-NetAdapterName Ethernet -AllowManagementOS $true
```

Para crear un conmutador interno, ejecute el siguiente comando.
```PowerShell
New-VMSwitch -name InternalSwitch -SwitchType Internal
```

Para crear un conmutador privado, ejecute el siguiente comando.
```PowerShell
New-VMSwitch -name PrivateSwitch -SwitchType Private
```

## Crear una VM en hyper-v
1. Para iniciar el proceso de creación de la máquina virtual debemos acceder como administradores a PowerShell y allí ejecutar la siguiente sintaxis:
```PoweShell
New-VM -Name “Nombre VM” -MemoryStartupBytes 6GB -BootDevice VHD -NewVHDPath Ruta.vhdx -Path “Ruta” -NewVHDSizeBytes 30GB -Generation 2 -Switch “Adaptador”
```

**Lista de comandos**

| Parámetro                   | Argumento     | Descripción                                                                                                               |
| --------------------------- | ------------- | ------------------------------------------------------------------------------------------------------------------------- |
|  New-VM                     |               |  Permite crear la máquina virtual                                                                                         |
| -Name                       | "Nombre"      |  Define el nombre de la máquina                                                                                           |
| -MemoryStartupBytes         | 6GB           |  Memoria RAM a asignar                                                                                                    |
| -BootDevice VHD -NewVHDPath | ruta.vhdx     |  Permite crear un nuevo disco duro virtual (\* .vhdx) en la ubicación deseada y establecerlo como dispositivo de arranque |
| -Path                       | “Ruta”        |  Permite definir la ruta donde se creará el disco duro                                                                    |
| -NewVHDSizeBytes            | 60GB          |  Tamaño a asignar al disco                                                                                                |
| -Generation                 | 1 o 2         |  Define la generación de la máquina a usar                                                                                |
| -Switch                     | "Adaptador"   |  Permite vincular el adaptador de red a la máquina virtual                                                                |

2. Redireccionar la imagen ISO del sistema deseado hacia la máquina virtual con el siguiente orden:
```PowerShell
Add-VMDvdDrive -VMName "Nombre" -Path D:\\Software\\Ubuntu\\ubuntu-19.10-desktop-amd64.iso
```

>La ruta debe ser definida donde esté alojada la imagen ISO.


| Parámetro         | Argumento        | Descripción                           |
| ----------------- | ---------------- | ------------------------------------- |
|  Add-VMDvdDrive   |                  |  Crea la unidad virtual de DVD        |
| -VMName           |    "Nombre"      |  Allí ingresamos la maquina a asociar |
| -Path             |    Ruta.path     |  Especifica la ruta de la imagen ISO  |

3. Ahora iniciamos la máquina virtual con el siguiente comando:
```PowerShell
Start-VM -Name "Nombre"
```

4. Nos conectamos a ella ejecutando:
```PowerShell
VMConnect.exe
```

## Cambiar resolución hyper-v en linux
Hyper-v tiene lo que se conoce como sesión mejorada, pero no es compatible con las distribuciones de linux (exceptuando ubuntu), para cambiar la resolución en las demás distribuciones debemos seguir los siguientes comandos: 

1- Modicar el archivo /etc/default/grub como usuario root:
```bash
sudo nano /etc/default/grub
```

2- Agregar la siguiente línea de comando: 
```bash
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash video=hyperv_fb:1920×1080″
```

3- Volver a compilar el grub:
```bash
sudo grub-mkconfig -o /boot/grub/grub.cfg
```

# Referencias Biblográficas
https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v
https://archlinux.org/
https://www.archlinux-es.org/
