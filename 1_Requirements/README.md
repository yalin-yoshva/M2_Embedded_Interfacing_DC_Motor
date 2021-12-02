# Requirements

In some of your electronic projects you may want to control a DC Motor with Atmega32 Microcontroller. We can’t connect a DC Motor directly to a microcontroller due to following reasons.

A microcontroller can’t supply the current required for the working of DC Motor. ATmega32 Microcontroller can source or sink currents up to 40mA but a DC Motor needs current very much more than that.
The negative voltages created due to the back emf of the motor may affect the proper functioning of the microcontroller.
You may need to control the direction of rotation of the motor by changing the polarity of  the motor supply.
The operating voltage of the DC Motor may be much higher than the operating voltage of the microcontroller.
DC Motor
To solve these problems you may use transistorized H Bridge in which freewheeling diodes are used to avoid problems due to back emf. Thus it requires minimum four transistors, diodes and resistors for each motor. It is better to use readymade ICs such as L293D or L293 instead of making your own H Bridge, which simplifies your project.

L293D is a Quadruple Half H-Bridge driver commonly used for motor driving. We needn’t connect any transistors, resistors or freewheeling diodes. All the four outputs of this IC are TTL compatible and output clamp diodes are provided to drive inductive loads.  L293D can provide up to 600mA current, in the voltage raging from 4.5 to 36v. L293 is a similar IC which can provide up to 1A in the same voltage range.

L293 or L293D contains four Half H Bridge drivers and are enabled in pairs. Input EN1  is used to enable pair 1 (IN1-OUT1, IN2-OUT2) and input EN2 is used to enable pair 2 (IN3-OUT3, IN4-OUT4). We can drive two DC Motors with one L293D, but here for demonstration we are using only one. You can connect second DC Motor to driver pair 2 according to your needs.


## DC Motor Controlling with ATmega328

# INTRODUCTION :
This activity is demonstration of controlling DC motor with the help of Atmega328 microcontroller.

In this activity, 
I performed two operations with DC motor
1) Controlling DC motor using in clockwise direction using switch.
2) Controlling DC motor direction( clockwise & anticlockwise ) using switch.

## RESEARCH



DC MOTOR: 
A direct current (DC) motor is a type of electric machine that converts electrical energy into mechanical energy. DC motors take electrical power through direct current, and convert this energy into mechanical rotation.
DC motors use magnetic fields that occur from the electrical currents generated, which powers the movement of a rotor fixed within the output shaft. The output torque and speed depends upon both the electrical input and the design of the motor.

Atmega 328:
The high-performance Microchip 8-bit AVR® RISC-based microcontroller combines 32 KB ISP Flash memory with read-while-write capabilities, 1 KB EEPROM, 2 KB SRAM, 23 general purpose I/O lines, 32 general purpose working registers, three flexible timer/counters with compare modes, internal and external interrupts, serial programmable USART, a byte-oriented Two-Wire serial interface, SPI serial port, 6-channel 10-bit A/D converter (8-channels in TQFP and QFN/MLF packages), programmable watchdog timer with internal oscillator, and five software selectable power saving modes. The device operates between 1.8-5.5 volts.


## SWOT Analysis

Strength : Gives experience of working with ATmega328 microcontroller and do simulation.

Weakness : Requires handson experience about Embedded programming and good knowlege about pin connection of Atmega 328 microcontroller.

## 4W's and 1'H
# 4W's

Who : Can be done by person having knowledge of embedded .

What : Do programming of microcontroller and perform simulation.

When :

Where : On the Laptop or PC .

# 1'H
How : Programming and simulation can be done on terminal and simulide from Personal computer or laptop.



## Detail Requirements :
## High Level Requirements :
| ID | Description | Status |
| --- | --- | --- |
| HLR_1 | The user can change its selected sign("ON","OFF"). | Implemented |
| HLR_1 | The user can on and off DC motor | Implemented |
| HLR_2	| atmega 328 Microcontroller used for the entire process |  Implemented |
| HLR_3 |	Source Code	Used for the Execute the system |  Implemented |


## Low Level Requiremnets :
| ID | Description | Status |
| --- | --- | --- |
| LLR_1 | List of operations displayed | Implemented |
| LLR_2 | Input from the user. | Implemented |
| LLR_3 |Exit the program . | Implemented |

