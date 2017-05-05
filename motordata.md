## Project 2 - Data-Sheets

## How to choose the motor-load combination?

The motor parameters will be assigned randomly, based on the last digit of your student number. For example if your student number is 1244839, then take the modulus 2 of the last digit:

mod-2 (9) = 1

Then you need to use the parameters of the Motor#1 for your project.

## Motor Data-Sheet

In this project, there will be 3 different applications where motor ratings, mechanical properties and load conditions will be different.

## Application-0: 1.8 MW Metro Taction System.

In this project, you are going to model a railway traction system. The underground metro systems consists of 3 carriages, with a mass of 42 tons each, and there are two motors driving each carriage. The specifications for each traction motor are as follows:

- Rated Power: 305 kW
- Rated Voltage: 463 V
- Max. Voltage: 700 V
- Rated Current: 720 A
- Max. Current: 1200 A (for 2min)
- Rated Speed: 600 rpm
- Max. Speed: 2000 rpm
- Rated Torque: 4812 Nm
- Armature Resistance: 0.058 Ω
- Armature Inductance: 4 mH 
- Back EMF constant: 6.68 V/rad/s (Normally, series wound DC motors are used in traction applications, but for simplicity assume a PM motor with constant field current is used throughout this project).
- Motor Inertia: 25 kgm²
- Axle Shaft Inertia: 15 kgm²
- Referred carriage inertia: 1200 kgm² (Actually, I didn't have to give this number, as you can calculate it if I say train moves at 54 km/h when the motor is rotating at 600 rpm. As a bonus, show the inertia calculation in your reports).


The specifications of the load side is as follows:

- The train moves on a flat track
- Friction coefficient: 7.5 Nm/rad/s (Referred to motor side, per motor)
- Rated train speed: 54 km/h (when rotor speed is 600 rpm)
- Acceleration limit: 0.8 m/s² 
- Deceleration limit: 1.0 m/s²
- Jerk limit: (0.8 m/s²)/s  (implement it as a bonus)

## Application-1: 4kW Elevator System.

In this project, you are going to model an elevator system as shown in the figure below. T

![250px](./elevator.png)

The elevator consists of a counterweight and connected to the motor side with a gearbox and pulley system.

The specifications of the elevator motor are as follows:

- Rated Power: 4 kW
- Rated Voltage: 360 V
- Rated Current: 12.78 A
- Max. Current: 20 A (for 3min)
- Rated Speed: 1800 rpm
- Max. Speed: 2000 rpm
- Rated Torque: 21.2 Nm
- Armature Resistance: 3.68 Ω
- Armature Inductance: 32 mH 
- Back EMF constant: 1.66 V/rad/s (PM DC motor)
- Motor+Gearbox Inertia: 0.05 kgm²
- Referred load inertia: 0.0512 kgm² (Actually, I didn't have to give this number, as you could calculate it using the dimensions given in the figure. Calculate it as a bonus in your report.).

The specifications of the load side is as follows:

- Neglect friction losses
- Carried mass: 400kg
- Elevator cabin mass: 100 kg
- Counterweight mass: 300 kg
- The gravitational load torque: 15.7 Nm (referred to the motor side)
- Cabin max. speed: 1.4 m/s (referred motor speed 1671 rpm)
- Acceleration time: 3s
- Deceleration time: 5s
