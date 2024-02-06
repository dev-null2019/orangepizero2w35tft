# Device tree overlay and xorg config files for a 3.5 inch SPI ili9486 display on the Orangepi Zero 2W

I used this display https://joy-it.net/en/products/RB-TFT3.5 - but I think the waveshare 35a has a similar pinout. Take a look at the pinout diagram! </br>
</br>
Steps to make it work:

git clone https://github.com/dev-null2019/orangepizero2w35tft</br>
cd orangepizero2w35tft</br>

sudo mv ./80-calibration.conf /usr/share/X11/xorg.conf.d </br>
sudo mv ./99-fbdev.conf /usr/share/X11/xorg.conf.d</br>
sudo orangepi-add-overlay ./joyit35a-overlay.dts</br>

add fbtft to /etc/modules</br>

reboot
