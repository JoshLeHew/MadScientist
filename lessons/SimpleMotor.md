# Electric Motor

DC (direct current) electric motors are great for adding movement to your projects.  Simple electric motors like the ones we will be using have only two connections.  Connect these wires to a power source and the motor will start moving.  Be careful though to use a power source that is appropriate for your motor. You don't want to burn out the motor with too much voltage. 

## N20 Electric Motor

<img alt="N20 Electric Motor" src="/lessons/images/motor.PNG" width="500"/>

We are using the GA12-N20 Motor.  They are metal geared high torque motors and can typically support from 3V up to 12V of power.  There are many versions of the N20 motors.  The ones we are using can turn about 100 RPM (revolutions per minute) at 3 volts.  The motors in your kit should not be used with more than 5 volts.  The Raspberry Pi Pico GPIO pins output 3.3 volts and can be controlled programmatically, but the VBUS pin outputs a steady 5 volts. However, the pins on the Pico are designed for very low power devices like LEDs or sensors and are not recommended to run electric motors.  So, caution needs to be taken when using electric motors with the Pico to not draw too much power (amps) through the board.  A small motor with little load (no resistance) should be fine for our quick test, but we will show you the correct way to power a motor using the Pico later.  For now, let's focus on understanding how simple electric motors work and just be sure there's nothing restricting your motor's movement during this lab; otherwise, you may release the [magic smoke](https://en.wikipedia.org/wiki/Magic_smoke) from the Pico.

## Try it out
To test our electric motor, we will simply plug our Pico in via USB which will immediately provide a steady 5 volts of power on the VBUS pin. We can use this to temporarily test our motor.

At this point, we are just using the Pico as simple battery source.  So, connect one wire from the motor to the VBUS pin and the other to a ground pin.  It doesn't matter which wire you connect from the motor to the VBUS versus to ground. You are just providing a flow of electricity through the motor.  It can spin in either direction depending on the way the power flows.

<img alt="Wiring Diagram for Motor" src="/lessons/images/simple_motor_bb.png" width="500"/>

As soon as you connect the wires of the motor to the Pico, you should see the motor spinning.  If you reverse the wires, you should see them spin in the opposite direction.  

## Resources

[Data sheet for N20 motor](https://abra-electronics.com/electromechanical/motors/gear-motors/mini-metal-gearmotors/ga12-n20-3v100.html)

[Another Data sheet for N20 motor](https://temperosystems.com.au/wp-content/uploads/2021/03/N20-Micro-Speed-Gear-Motor.pdf)



