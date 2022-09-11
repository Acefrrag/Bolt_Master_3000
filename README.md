# Bolt Master 3000

## Repository Description
This github repositories collects all the documentation(CAD files, reports, BOMs, brainstorming notes) produced during the design and development of a proof-of-concept mechatronic system for the undergraduatee course MECA140 - Introduction to Engineering Design and Automation during A.Y. 2019-2020.

## Project Description

The aim of the proof-of-concept system was to explore ways to automatize the process of checking proper bolt installation on a generic structure.

The proof-of-concept system objective is to test the proper installation of 4 bolts in 1/4-20 holes on a 4-by-4-inch-area stainless steel plate. The system ensures bolt preload is present on all of them, and warns the user if a bolt is missing or not tightly screwed.

My team designed the Bolt Master 3000. This PLC-controlled system includes the OMRON NX1P2, which controls the actuation and the sensing system. 

### Working princple
The bolt is checked by pushing a DC motors onto it using a pneumatic actuator. The DC motor shaft is coupled with with a universal socket to successfully target the bolt cap. The DC motor starts applying a torque on the bolt and, depending on the amount of current drained from the power supply (measured with a shunt resistor), the controller is able to tell wheather the bolt is there or not.

Here is a demo of the system where it shows the system testing a correctly installed bolt and a missing bolt.

https://user-images.githubusercontent.com/59066474/189550218-b4baf25a-3ad1-4a13-9e47-b2368a44c600.mp4

The user interface on the screen has a button to start the bolt testing. The user interface displays the result with a pair of LEDs per bolt(RED for failure, GREEN for success). Neverthless, as it can be seen the user interface implemented included only 2 bolt. There was a lack of actuators and ther is only one DC motor testing unit. The corresponind is diplayed on the top right.

1. In the first test there is no bolt installed in the hole. As the motor spins, the amount of current drained is the lowest, therefore the system detects there is no bolt. The result is marked with a RED flag on the PLC monitor, aknowledging the failure in the installation of the bolt.
2. In the second test the bolt has been correctly installed. In this case as the voltage at the DC motor ends, the motor doesn't spin draining a much greater amount of current. In this case, the system detects a bolt and the corresponding GREEN LED light up.

### Phases of the Design

The design flow was supervised by the lecturer and consisted in different steps:

1.
2.
3.

## Team 

The project is the result of the team work with my teammates R.L. and A.J. 
