## Light Control Experiment
In this experiment we will control LED light state.

## Components Used
1. LED 
2. Breadboard
3. Jumper Wires
4. Resistor (220ohmx1)
5. ESP32 Wrover
6. GPIO Extension Board

## Hardware
All the components are connected as shown in the below figure.

## Process
- Open the menu config by typing in the following commands

    `cd ~/projects/Anjay-esp32-client`

   `idf.py menuconfig`


- Next navigate to component config 

- Select anjay-esp32-client.

- Select light control and is enabled.

- Next  navigate to light control options, enable the red light and entered the port number.( I have used 

- Later build the code

  `cd ~/projects/Anjay-esp32-client`
 
   ` idf.py build`
 
 - Finally flash the code by typing in the following commands.
 
     `cd ~/projects/Anjay-esp32-client`
 
    `sudo chmod 666 /dev/ttyUSB0`

     `idf.py -p 0 flash`

