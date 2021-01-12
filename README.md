WanderOS
===
Sistema desarrollado originalmente como proyecto de la clase 'Sistemas Operativos II' de la carrera de Ing. en sistemas de la UNAH

WanderOS es un sistema operativo basado en Arch Linux, elaborado con Archiso. El objetivo del mismo es tener un sistema enfocado al desarrollo en general, eliminando la molesta necesidad al desarrollador de configurar su sistema operativo para comenzar a trabajar.

Dado dicho objetivo, esperamos que aquella persona que instale WanderOS en su ordenador comience a trabajar inmediatamente y si necesita configurar algo, sea lo minimo posible.

Desktop
![Desktop_WanderOS](https://raw.githubusercontent.com/JeanlucBoquin/WanderOS/main/img/EscritorioWander.png "Desktop")

---
Calamares
![Desktop_WanderOS](https://raw.githubusercontent.com/JeanlucBoquin/WanderOS/main/img/CalamaresWander.png "Desktop")

Entorno de escritorio
---
**XFCE4** personalizado

Gestor de usuario
---
**sddm** personalizado

Consideración
---
WanderOS esta enfocado al desarrollo y cuenta con las herramientas necesarias para dicho objetivo, pero WanderOS puede ser utilizada por cualquier persona, no necesariamente un desarrollador.

Dado que cuenta con un abanico de programas lo suficientemente amplio para ser utilizado por el usuario común como un sistema operativo del día a día.

Lenguajes soportados
---
- C
- Java
- JavaScript
- PHP 
- Python

Herramientas
---
- MariaDB
- Qt5
- IDE Arduino
- Node-red
- netbeans
- Entre muchas mas

Instruciones:
---
Realizar los siguientes pasos como usuario root.
- git clone https://github.com/JeanlucBoquin/WanderOS.git
- mkarchiso -v -w WanderOS/work -o WanderOS/out WanderOS/
- run_archiso -i WanderoS/out/wanderos-yyyy.mm.dd-x86_64.iso
En caso que el ultimo comando les marque error "qemu"

pacman -S qemu
