# Linux Guide

My personal guide in installing Linux.

## Creating a bootable USB drive using USBImager

1. Download [USBImager](https://gitlab.com/bztsrc/usbimager)
2. Download Linux `.iso` installer
3. Open a terminal, navigate to the downloads folder and verify file integrity using `sha256sum filename.iso` and compare checksum from the official website.
4. Write the `.iso` file in a flashdrive using USBImager.

## Creating a bootable USB drive in Linux

1. Download Linux `.iso` installer
2. Open a terminal, navigate to the downloads folder and verify file integrity using `sha256sum filename.iso` and compare checksum from the official website.
3. Enter the following in the terminal
    ```sh
    sudo dd if=Downloads/linux.iso of=/dev/sda bs=4M status=progress && sudo sync
    ```

## Linux Distros Guide

- [Arch Linux](./Distros/ArchLinux.md)
- [Debian](./Distros/Debian.md)
- [CachyOS](./Distros/CachyOS.md)
- [Raspberry Pi OS](./Distros/RaspberryPiOS.md)
- [NixOS](./Distros/NixOS.md)
