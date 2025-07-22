# Stinger

[![Discord](https://img.shields.io/discord/1318280486107480064?style=for-the-badge&logo=discord&logoColor=white&label=Discord&color=5765F2)](https://discord.gg/RR9ZNNtcx3)

-   Documentation can be found in the [Wiki](https://github.com/bastian2001/Stinger-Docs/wiki)
-   For building your own stinger, check out the [Assembly Guide](https://github.com/Project-Stinger/Stinger-Docs/blob/main/StingerV2AssemblyGuide.pdf). Hardware kits and a video will be available soon.
-   If you want to join the community or have questions, the best place to ask is the [Discord server](https://discord.gg/RR9ZNNtcx3). Alternatively, you can also use the [GitHub Discussions](https://github.com/bastian2001/Stinger-Docs/discussions).
-   3D print models are available in the [3D Models](#) directory, and you can find the OnShape CAD files [here](#).

# Spec Sheet

Dual stage brushless design (190-230fps)
Solenoid firing (+30dps)
6S powered, 4S compatible with lower firing rates
Full closed loop control of motor RPM and solenoid position
Modular stock and front BCAR
Fully configurable menu with joystick and display
Magazine detection sensor
Tournament mode
Dynamic motor idling by gyro
Multiple firing modes and up to 5 user presets
Aluminum sides for motor cooling
Dimensions (approx): H=181mm, L=263mm (picatinny stock), W=28mm (very thin)
Uses Worker Talon (and similar) magazines
Sleep mode after inactivity

# About

Stinger (V2) is an advanced dart blaster, shooting short darts such as Worker HE. It uses 4 BLDC motors, which are each controlled with a fast PID loop to ensure good matching and fast spinup times, driven by an AM32 ESC. A solenoid, driven in closed loop controlled rapid decay for fast fire rates, drives the darts into the flywheels. The blaster is entirely configurable, from firing motor RPM, to firing modes, multiple user modes, tournament mode... (see (insert software repo link)) for more info.

To keep the motors cool and for structural reasons the blaster is a metal 'sandwhich', the motors are mounted to the aluminum side panel where they can dissapate heat.

Multiple BCAR* and stock modules** offer flexibility in accuracy and playing styles
*BCAR (Bearing Centered Auto-Rotating) does 2 things. It stabilizes the rear of the dart as it comes out of the barrel (check initial video) causing less random drag, and it provides spin to the dart which then gyroscopically stabilizes it like rifling in a barrel. Right now 3 modules exist, Low Crush (2.7mm), High Crush (3.0mm) and nobcar.
**Current stock modules include: folding stock (with carbon fiber rods), locking stock (same rod system), and picatinny stock. But more can be designed in the future.

A custom PCB (insert pcb repo link) houses all the input/output devices, controlled by an RP2040. It also has a high side switch to enter sleep mode. In sleep mode, the ESC is turned off to conserve energy, but the blaster still uses some energy to detect movement and run the code so do not leave it off for too long.

Stinger was developed entirely here in the EU by Bastian and me (Stan). Bastian is responsible for the PCB and code development and I did the rest.

After the 'launch' on youtube, 47 Stinger V2's were sold as finished blasters to all over the world, but mostly the US. This was quite an experience and we learned a lot from it. Now it is time for everyone to have access to this wonderful project. 

