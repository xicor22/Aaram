# Aaram
PCB design for retro fitting old switch boards with new tech to control it remotely.

## Features
1. Controls 4 loads using
  - 1 Triac using Phase angle control
      > Note: Triac circuit has added protection for the back EMF generateed by inductive load like fan.
  - 3 Relays for controlling other loads
      > Try not use heavy inductive load using relays. During testing, the MCU was bugging out when load was switched.
2. Input from switches.
      - To reduce rewiring the whole switch board, directly connect the rocker switch output terminal to the input provided on the board.
      - The voltage divider reduces thee voltage, then the diode give a half sine wave which is smoothed out by the capacitor. The final voltage is read by the quad channel opto which tells the ESP about the switch state.
3. Uses ZMCT103C current sensor for current measurement.
4. Uses DHT22 for temperature and humidity sensor.
5. 8 Spare pins for additional functionality.

## Images
|View|Image|
|----|-----|
|1<sup>st</sup> Layer| ![Layer 1](/asset/l1.jpg)|
|2<sup>nd</sup> Layer| ![Layer 2](/asset/l2.jpg)|
|3<sup>rd</sup> Layer| ![Layer 3](/asset/l3.jpg)|
|3D view| ![Layer 4](/asset/3d.jpg)|
