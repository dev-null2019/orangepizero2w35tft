# Device tree overlay and xorg config files for a 3.5 inch SPI ili9486 display on the Orangepi Zero 2W

Steps to make it work:

git clone https://github.com/dev-null2019/orangepizero2w35tft
cd orangepizero2w35tft

sudo mv ./80-calibration.conf /usr/share/X11/xorg.conf.d 
sudo mv ./99-fbdev.conf /usr/share/X11/xorg.conf.d
sudo orangepi-add-overlay ./joyit35a-overlay.dts


add fbtft to /etc/modules


reboot
