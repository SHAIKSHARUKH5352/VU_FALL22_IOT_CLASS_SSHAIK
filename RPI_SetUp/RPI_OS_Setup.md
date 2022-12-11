## RPIOS-Setup

I have done the following things during the class. 
- I have downloaded balena etcher, Diet Pi Disk Image and 7 zip through the links given by professor.
- Using the 7 zip I have extracted the Diet Pi files and then I have dropped the extracted Diet Pi files in balena etcher to flash it.
-  In the balena etcher, insert SD card is inserted and select it as target. 
-  If it was unable to detect the SD card ,  do it multiple times till you see the contents of the card.

## Changes to dietpi.txt and dietpi-wifi.txt

- Copy Dietpi.txt and Dietpi-Wifi.txt to a temporary directory.
- Add the router's SSID and login information to dietpi-wifi.txt
- Add current location and Wi-Fi network default settings to dietpi.txt. 
- Later make the following changes in dietpi-wifi.txt 

```
aWIFI_SSID[0]=''  - Updated it to my SSID 
aWIFI_KEY[0]=''   - Updated it to my password .
```

- Later make the following changes to dietpi.txt

```
AUTO_SETUP_LOCALE=en_US.UTF-8
AUTO_SETUP_KEYBOARD_LAYOUT=us
AUTO_SETUP_TIMEZONE=America/New_York
AUTO_SETUP_NET_ETHERNET_ENABLED=0
AUTO_SETUP_NET_WIFI_ENABLED=1
AUTO_SETUP_NET_WIFI_COUNTRY_CODE=US
AUTO_SETUP_DHCP_TO_STATIC=1
AUTO_SETUP_NET_HOSTNAME=DietPi_SSHAIK
AUTO_SETUP_HEADLESS=1
AUTO_SETUP_AUTOSTART_TARGET_INDEX=1
SURVEY_OPTED_IN=0
CONFIG_SERIAL_CONSOLE_ENABLE=1

```

- Lastly, eject the SD card from the laptop.
- After all this process, start setting up Raspberry Pi. 

## Setting up RaspberryPi

- Insert the sd card in the Raspberry Pi. 
- Check if there are red and green lights that  flashing. 
- After few minutes  you'll see the green light stops flashing. 
- Now check if dietpi's wifi address is visible in the admin portal.
