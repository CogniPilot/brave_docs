# About Brave Bennu (COMING SOON)

[Bennu](https://en.wikipedia.org/wiki/Bennu) is an ancient Egyptian deity linked with the Sun, creation, and rebirth. Typically shown in depictions as a heron like bird wearing a crown, Bennu is believed to have been the original inspiration for the phoenix legends that developed in Greek mythology.

**Brave Bennu** represents the next evolution of CogniPilot's light weight, and minimalistic software stack following a correct by construction software paradigm.

## Correct by Construction Design Drivers

CogniPilot is not aiming to re-invent an opensource autopilot that can be a drop in replacement for use in Hobby drones, FPV Racing drones, or a wide variety of DIY autonomous vehicles, there are many great autopilots for that ([ArduPilot](https://ardupilot.org/), [BetaFlight](https://betaflight.com/), [PX4](https://px4.io/)). CogniPilot instead focuses on state-of-the-art methologies for creating an autopilot with mathematically provable robustness properties. In order to achieve this level of reliability, accurate mathematical models of the vehicle and control software must be established that are beyond the expected domain of many hobbyists. However, for those willing to pursue the extra steps to create a mathematical model of their vehicle, templates are available to enable out of tree custom vehicles. CogniPilot is a new class of open source autopilot that can conduct safety critical missions such as public transport, with a level of safety assurance not currently available in other open source autopilots.

  * **Minimum Viable Code for the Mission**: By minimizing the lines of source code and branching, CogniPilot ensures higher reliability, maintainability, and verifiability of the project. 

  * **Minimize Branch Statements in Control and Estimation Code**: CogniPilot generally classifies its code components into two areas. The first is low-level driver and application code. The second is guidance, control, and estimation code for the vehicle. Developers carefully consider the addition of each branch (if statement etc.) in the code for the estimator and controller, as developers are modelling the entire system mathematically. Each branch statement considerably complicates the verification task.

  * **Minimize Maintenance to Maintain Reliability**: A goal of CogniPilot is to support a wide variety of vehicles (Planes, Copters, Boats, Rovers, Submersibles) and user applications while maintaining software integrity and reliaiblity. CogniPilot plans to limit official support for each release to a minimal amount of vehicles for each class, while providing out of tree support via templates.

  * **Deprecate if No-longer Maintained**: On each release cycle, the CogniPilot technical steering committee (TSC) will make a decision on whether to maintain official support for each vehicle platform or whether to adopt a new platform. This is to combat the slow creep in lines of code due to vehicle specific edge cases. 


## Software Stack
* Ubuntu 24.04
* Zephyr RTOS 3.7+
* ROS 2 Jazzy
* Gazebo Harmonic

## Currently supported platforms

### Rover
   * [B3RB](./reference_systems/b3rb/about.md)
   * ELM4
   * MELM
### Multirotor
   * RDD2

## Get started

To get started follow the guide on [how to install on a computer](./getting_started/install.md).

## CogniPilot's next release
To still be named, but going by C-Mythical (a mythical creature with a name starting with C) will have planned additional support for:

### Multirotor
   * TBD
### Submersible
   * TBD
### Plane
   * TBD



