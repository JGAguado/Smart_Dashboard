:term:`FAQ`
=============================

After connecting the battery, I don't see the e-paper refresh or any LED on.
    The two LEDs that are on the board (STDBY & CHRG) only indicate the state of the battery while charging (USB-C or solar panel). The way to 
    check if the board is alive is pressing the Reset pushbutton and see that the e-paper refreshes correctly. If not, you will need to 
    charge the battery through the USB-C. 

After connecting the battery and the USB power I see the both LED (STDBY & CHRG) on.
    Check the battery connection polarity: red with + and black/blue with -. 
    Since there is no standard relative to the JST connectors polarity, please pay 
    special attention when connecting any battery to the board. 

Can I upload ESPHome directly from the Home Assistance setup running on my Raspberry Pi?
    Yes you can, and actually this is one of the simplest and more effective way to upload ESPHome.

Can I upload firmware through the USB-C?
    Yes, the ESP32-S2 includes a full-speed USB On-The-Go (OTG) interface to enable USB communication.

When I try to compile the given YAML and upload it into the board I get some error messages saying that I miss some files (Audiowide.ttf, icon-map.h, etc). How to fix it?
    Just the configuration YAML file isn’t enough and you might get an error asking for missing items (the fonts and the images). The reason is because
    on the configuration we are asking for some files (the fonts that you want for the digits or the icons and the background image with the plant and the gauges).
    
    Therefore you need to upload into the folder with the configuration YAML file the required files. I strongly suggest to use Visual studio code and just drag and 
    drop the items according to the structure mentioned on the :ref:`esphome` programming section.

Can I use it if there is no internet connection? 
    Technically yes, the ESP32 can work without internet, but since the main strength of this board is to present data, you will still need internet to gather 
    certain data (weather forecast, stock prices, etc.). However, if you use Home Assistant it is possible that the data you want to present comes from local 
    sensors you have, in this case internet may not be that required.

Can the Smart Dashboard be used outdoor? 
    No, it wasn't designed for such case scenario. In addition, take into account that e-paper displays degrades under direct UV light exposure. 

What is battery life on single charge?
    With the ESPHome configuration YAML, (10s working and e-paper update, and 1h on deep sleep mode) the expected battery life is around 40-50 days for 
    the recommended 5000mAh LiPo. 

Can I attach a solar panel to extend the battery?
    Yes, there are two unsoldered pins marked as +/- where you can attach a 5V solar pannel of your choice. 
    Just make sure the sun exposed area is the solar panel and not the e-ink display.

