# Raspberry Pi OS

My personal guide to install Raspberry Pi OS on a Raspberry Pi board.

Official website: https://www.raspberrypi.com

## 1. Preparation

Download Imager
https://www.raspberrypi.com/software

I recommend installing Lite (headless, no DE) and make sure to setup SSH.

## 2. Installation

Installation is straightforward. Just insert Micro SD card to the Rapsberry Pi.

## 3. Post Setup

```bash
sudo apt update
sudo apt upgrade
```

```bash
sudo rfkill block wifi
sudo rfkill block bluetooth
```

```bash
sudo nano /etc/ssh/sshd_config
```

```bash
sudo systemctl restart sshd
```

```bash
sudo apt install ufw
```

```bash
sudo ufw allow from IP-ADDR to any port PORT
```

```bash
sudo ufw enable
sudo systemctl enable --now ufw
```

### Fastfetch

```bash
sudo apt install fastfetch
```

```bash
fastfetch --gen-config
```

### Docker

https://docs.docker.com/engine/install/debian

```bash title:"Add user to docker group then logout and login"
sudo usermod -aG docker $USER
```
