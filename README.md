# rasp-zero-w-shairport-sync
Setup shairport-sync on a Raspberry Zero W

## Prepare OS

1. Plug the SD card into your computer
1. Download Raspberry Imager from https://www.raspberrypi.org/software/
1. Start Raspberry Imager and select "Raspberry Pi OS (other)" and "Raspberry Pi OS Lite (32-bit)"
1. Select your SD card
1. Click on the gear icon and select "Advanced Options"
1. Check "Set hostname" and enter a hostname, e.g. "hifi.local"
1. Check "Enable SSH" and set a username and password
1. CHeck "Configure Wireless LAN" and enter your WiFi credentials
1. Click on "Write" and wait for the process to finish

## Install Software

1. Plug the SD card into your Raspberry Pi
1. Wait until the Raspberry Pi is up and running and connected to your WiFi
1. Connect to the Raspberry Pi via SSH
    ```bash
    ssh username@hostname
    ```
1. Update the system
    ```bash
    sudo apt update
    sudo apt upgrade
    ```
1. Install shairport-sync
    ```bash
1. Install docker
    ```bash
    curl -fsSL https://get.docker.com -o get-docker.sh
    sudo sh get-docker.sh
    ```
1. Install git
    ```bash
    sudo apt install git
    ```
1. Clone this repository
    ```bash
    git clone https://github.com/linobino1/rasp-zero-w-shairport-sync.git
    ```
1. Change into the repository directory
    ```bash
    cd rasp-zero-w-shairport-sync
    ```
1. Build the docker image
    ```bash
    docker compose up
    ```