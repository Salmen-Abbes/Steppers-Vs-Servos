# Servos vs. Steppers
Welcome to the Servos vs. Steppers Repository. Delve into the world of motor dynamics, as we navigate through the nuances of servo and stepper motors. Gain insights on selection, applications, and unleash the power of precision in robotics and electronics.

## Stepper Motors

### Definition

Stepper motors are precise electromechanical devices that convert digital signals into incremental rotation, delivering precise control over angular position. Composed of multiple coils, they move in discrete steps, making them ideal for applications requiring accurate positioning, such as 3D printers, CNC machines, and robotics.

In other words, we can lean on Stepper motors in handling precises movements and not into speed of rotation.

### Torque Spec

Stepper motors are also known for their "Power Lifting" ability, as they are able of carrying weight while rotating.

Here, I want to talk about the "Torque" property, so basically Torque in motors refers to the rotational force or moment of force that a motor can exert. It is a measure of the motor's ability to generate rotational motion and is typically represented in Newton-meters (Nm) or ounce-inches. So, higher torque values signify greater rotational force, crucial for overcoming resistance or inertia in mechanical systems.

To make it more simple, let's consider the torque as the capabilty of the motor in holding weights. Below, this image illustrates what the torque is ( Do not worry, most of the times we don't have to calculate the torque of a motor as it is given among the specs of motors when buying)

![image](https://github.com/Salmen-Abbes/Steppers-Vs-Servos/assets/114873030/0a4d160b-58b7-4c41-960a-1bf8dc9fee52)

### Internal Sturcture

Now, let's dive into the stepper motor infra-structure, unlike traditional motors, a stepper motor consists of multiple coils and a rotor with teeth. The rotor is magnetized, and the stator, comprising coils wound around poles, generates magnetic fields. The motor operates by dividing a full rotation into a series of discrete steps. As each coil is energized sequentially, it induces magnetic attraction or repulsion, causing the rotor to move incrementally. The number of steps per revolution defines the motor's precision. 

![STEPPER-2](https://github.com/Salmen-Abbes/Steppers-Vs-Servos/assets/114873030/1d0a853f-a56d-433c-8b56-0fbb8d738c5b)

To calculate the step angle of a stepper motor, we can apply the following formula : Step angle = 360 / Steps per Revolution, example a motor has 200 Steps/revolution ( it means it achieves 200 steps in a complete tour of 360°) , then the step angle equals to 360 / 200 which is almost 1.8° ( in most of stepper motors ).

### Control

Controlling a stepper motor can't be done directly through a Dev board as it requires a specific module called a stepper motor driver. Stepper motor drivers provide the same main functionality ( which is controlling a stepper motor ) but are quite different in usage , such as current acceptance, Dev card compatibility, pinout, number of steppers connected...

So it is up to you to choose the right driver for the usage you want ( please note that the examples provided are only the most used ones, you can find another drivers that can suit you better ) :

![image](https://github.com/Salmen-Abbes/Steppers-Vs-Servos/assets/114873030/30a4d829-4cd0-493e-9029-ca3baf3fdc5c)


### Examples of Stepper Motors

There is a variety of Stepper Motors types, but the most known one is the 'Nema' size setppers. Nema stepper Motors are generally affordable and provide a quite respectable performance.

Nema Stepper Motors are classified by frame size, which is the reference indexed in the name of the motor , Nema "X" ( example Nema 17 has a frame size of 1.7 inch )

And this is a table illustrating some specs of Nema size Stepper Motors:

![image](https://github.com/Salmen-Abbes/Steppers-Vs-Servos/assets/114873030/26e3b686-d9cf-4c4c-baa5-8b8cfe344898)


