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


