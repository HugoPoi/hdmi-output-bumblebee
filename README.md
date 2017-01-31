# Scripts to enable HDMI Output with bumblebee

This script help to enable and disable interfaces on Optimus devices which are physicaly on nvidia GPU like Asus U36 laptop.
This [blog
post](http://www.unixreich.com/blog/2013/linux-nvidia-optimus-on-thinkpad-w520w530-with-external-monitor-finally-solved/) help me to write the scripts.

##Requirements
* Bumblebee installed and working
* The intel-virtual-output utility

##Install

1. `mv /etc/bumblebee/bumblebee.conf /etc/bumblebee/bumblebee.default.conf`
1. `ln -s /etc/bumblebee/bumblebee.default.conf /etc/bumblebee/bumblebee.conf`
1. `cp ./bumblebee.hdmi.conf /etc/bumblebee/bumblebee.hdmi.conf`
1. `cp ./xorg.config.nvidia.hdmi /etc/bumblebee/xorg.config.nvidia.hdmi`
1. You may need to adapt the `bumblebee.hdmi.conf` accordling to your
   setup

##Usage
1. Enable Hdmi `./enable-hdmi`
1. Disable Hdmi `./disable-hdmi`

##More Info
* Tested with Ubuntu 14.04 and nvidia-340.
* `bumblebee.default.conf` is provided for example

