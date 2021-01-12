Imagenes de error durante el desarrollo


![Error](https://raw.githubusercontent.com/JeanlucBoquin/WanderOS/main/img/imgError/error-bootloader.jpg "Error_bootloader")
Agregar el paquete grub en el archivo packages.x86_64

---

![Error](https://raw.githubusercontent.com/JeanlucBoquin/WanderOS/main/img/imgError/error-update-initramfs.jpg "Error_initramfs")
Comentar "initramfs" del archivo airootfs/etc/calamares/settings.conf (valido para sistemas basados en debian)

---

![Error](https://raw.githubusercontent.com/JeanlucBoquin/WanderOS/main/img/imgError/error_mkinitcpio.jpg "Error_mkinitcpio")
Modificar linux312 por linux del archivo airootfs/etc/calamares/modules/initcpio.conf 

---

![Error](https://raw.githubusercontent.com/JeanlucBoquin/WanderOS/main/img/imgError/error_unsquash.jpg "Error_unsquash")

unpack:
    -   source: "/run/archiso/bootmnt/arch/x86_64/airootfs.sfs"
        sourcefs: "squashfs"
        destination: "/"
    -   source: "/run/archiso/bootmnt/arch/boot/x86_64/vmlinuz-linux"
        sourcefs: "file"
        destination: "/boot/vmlinuz-linux"