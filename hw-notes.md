---
layout: page
title: HW-notes
permalink: /hw-notes/
---

# Bring-up Raspberry Pi 2 (model B) and Raspberry Camera v2 (02/25/18)

1. Checkout the required parts at **[raspi](https://www.raspberrypi.org/)** website to kick-off.
2. The camera has two versions - NoIR and IR version. For general purpose use
prefer the IR version. The difference between the two being the software IR filter
applied between the two sensors.
3. The camera v2 is based of the **[sony IMX219](https://www.sony-semicon.co.jp/products_en/new_pro/april_2014/imx219_e.html#Figure1)** sensor - checkout the product
page for more details.
4. Connect the camera to the raspi. Follow the instructions from the video below.
**[raspi-connect-to-camera-v2](https://www.youtube.com/watch?v=T8T6S5eFpqE&)**
5. Connect the HDMI cable before the power-up.
6. Attach a **[EdiMax-wifi-dongle]()**. You would have to make changes to the /etc/network/interfaces to connect the
wifi dongle to your wifi. Follow the steps given **[here](https://raspberrypihq.com/how-to-add-wifi-to-the-raspberry-pi/)**. Ran into a couple of issues. Some silly, some that took some time.
    - Had typos ahead of # in the /etc/network interfaces.
    - After running the 'sudo service networking reload', got an error saying couldn't 'ifup: no interface(s specified)'. Had to manually enter the interface mapping in /run/network/ifstate. **[Reference](https://unix.stackexchange.com/questions/50602/cant-ifdown-eth0-main-interface)**
7. After all goes good. Capture a still image with raspi using the command - 'raspistill -o image.png'. A small preview window will open. Smile big ... might be your first raspi-cam installation. ;) After 5 secs an image will be dumped to **image.png** file.
8. Start ssh dameon on the raspi - 'sudo service ssh start'.
9. pi ip - 'hostname -I'
10.
