I have done the following things during the class. First I have downloaded balena etcher, Diet Pi Disk Image and 7 zip through the links given by professor.

Using the 7 zip I have extracted the Diet Pi files and then I have dropped the extracted Diet Pi files in balena etcher to flash it. I haven’t gotten 
sd card and Raspberry Pi so I worked with Alekhya, Jaswanth, Mudith and Susmitha for the rest of the process. In the balena etcher, SD card is inserted and 
selected as target. First it was unable to detect the SD card so we had to do it multiple times and finally we were able to see the contents of the card.

Dietpi.txt and Dietpi-Wifi.txt were copied to a temporary directory. The router's SSID and login information were added to dietpi-wifi.txt, and the 
current location and Wi-Fi network default settings were added to dietpi.txt. I was successful in finishing the classwork up until this point. 

Later at home , I flashed the SD card . After the flash is successful I have made the following changes in dietpi-wifi.txt 
aWIFI_SSID[0]=''  - Updated it to my SSID 
aWIFI_KEY[0]=''   - Updated it to my password .

Later I made the following changes to dietpi.txt

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

Lastly... I ejected the SD card from my laptop.

After all this process, I started setting up my Raspberry Pi. First I inserted the sd card in the Raspberry Pi. There were red and green lights that were 
flashing. After few minutes the green light stopped flashing. Later dietpi's wifi address was visible in the admin portal.
