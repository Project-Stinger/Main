# Stinger

[![Discord](https://img.shields.io/discord/1318280486107480064?style=for-the-badge&logo=discord&logoColor=white&label=Discord&color=5765F2)](https://discord.gg/RR9ZNNtcx3)


-   Documentation can be found in the [Wiki](https://github.com/Project-Stinger/Main/wiki)
-   For building your own stinger, check out the [Assembly Guide](https://github.com/Project-Stinger/Stinger-Docs/blob/main/StingerV2AssemblyGuide.pdf). Hardware kits are available [from IFB](https://ifb.sg/products/project-stinger-v2), and assembly videos will come soon.
-   If you want to join the community or have questions, the best place to ask is the [Discord server](https://discord.gg/RR9ZNNtcx3). Alternatively, you can also use the [GitHub Discussions](https://github.com/Project-Stinger/Main/discussions).
-   3D print models are available in the [3D-Files repository](https://github.com/Project-Stinger/3D-Files), and you can find the OnShape CAD files [here](https://cad.onshape.com/documents/ffcb080386f1b38e45048950/w/111deafb99be991b56406227/e/2f9053495b44df3bf5ec6d73?renderMode=0&uiState=68cc3c6873af9957c3936df9), makerworld page [here](https://makerworld.com/en/models/1807037-stinger-v2-dual-stage-brushless-nerf-blaster#profileId-1927480)

# Spec Sheet

-   Dual stage brushless design (190+ fps)
-   Solenoid firing (30+ dps)
-   6S powered, 4S compatible with lower firing rates
-   Full closed loop control of motor RPM and solenoid position
-   Modular stock and front BCAR
-   Fully configurable menu with joystick and display
-   Magazine detection sensor
-   Tournament mode
-   Dynamic motor idling by gyro
-   Multiple firing modes and up to 5 user presets
-   Aluminum sides for motor cooling
-   Dimensions (approx): H=181mm, L=263mm (picatinny stock), W=28mm (very thin)
-   Uses Worker Talon (and similar) magazines
-   Sleep mode after inactivity

# About

Stinger (V2) is an advanced dart blaster, shooting short darts such as Worker HE. It uses 4 BLDC motors, which are each controlled with a fast PID loop to ensure good matching and fast spinup times, driven by an AM32 ESC. A solenoid, driven in closed loop controlled rapid decay for fast fire rates, drives the darts into the flywheels.

The blaster is entirely configurable, from firing motor RPM, to firing modes, multiple user modes, tournament mode... See the [software repository](https://github.com/Project-Stinger/Firmware) for more info.

To keep the motors cool and for structural reasons the blaster is a metal 'sandwich', the motors are mounted to the aluminum side panel where they can dissapate heat.

Multiple BCAR\* and stock modules\*\* offer flexibility in accuracy and playing styles

<details>
*BCAR (Bearing Centered Auto-Rotating) does 2 things. It stabilizes the rear of the dart as it comes out of the barrel (check initial video) causing less random drag, and it provides spin to the dart which then gyroscopically stabilizes it like rifling in a barrel. Right now 3 modules exist, Low Crush (2.7mm), High Crush (3.0mm) and nobcar.
\*\*Current stock modules include: folding stock (with carbon fiber rods), locking stock (same rod system), and picatinny stock. But more can be designed in the future.
</details><br>

A [custom PCB](https://github.com/Project-Stinger/Electronics) houses all the input/output devices, controlled by an RP2040. It also has a high side switch to enter sleep mode. In sleep mode, the screen and ESC are turned off so the battery does not drain as quickly during the matches.

Stinger was developed entirely here in the EU by Bastian and me (Stan). Bastian is responsible for the PCB and code development and I did the rest.

After the launch on YouTube, 47 Stinger V2's were sold as finished blasters to all over the world, but mostly the US. This was quite an experience and we learned a lot from it. Now it is time for everyone to have access to this wonderful project.

## Are you missing something?

Stinger is designed to be an open platform, so if you have an idea of a feature, head over to our Discord server, and post it there. We want Stinger to be the ultimate dart blaster. If you have an idea how to do the improvement yourself, you can do so in the respective repository.
