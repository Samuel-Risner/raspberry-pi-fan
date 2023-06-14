# raspberry-pi-fan

How I wired up my fan to my raspberry pi.

# Circuit

In the circuit the fan was replaced with a buzzer.

![Image of the circuit](circuit/circuit.png "circuit")

# Build

How my finished build looks:

![Image of finished build](build/build.jpeg "finished build")

The wire coloring matches the one on the circuit.

# How to configure the fan

1. Open a terminal on the pi
2. Enter ```sudo raspi-config```
3. Go to the fort option ```4 Performance Options```
4. Go the next forth option ```P4 Fan```
5. Select ```<Yes>``` for the option ```Would you like to enable fan temperature control?```
6. Enter your GPIO pin, in this case 2
7. Select ```<Ok>```
8. Enter the temperature at which your fan will turn on. NOTE: The fan will only turn off if the temperature is below 10°C of the value you entered.
9. Select ```<Ok>```
10. Confirm the following ```The fan on GPIO <your pin> is enabled and will turn on at <your temperature> degrees Celsius``` with ```<Ok>```
11. Select ```<Finish>``` to save
12. select what you want when you see ```Would you like to reboot now?```
