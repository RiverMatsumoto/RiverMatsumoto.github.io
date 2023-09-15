---
layout: project
type: project
image: img/rover/rover.png
title: "Teleoperated Rover"
date: 2023
published: true
labels:
  - C/C++ 
  - ROS
  - Python
  - Electronics
  - Git
summary: "A teleoperatable rover I built that collects data for terramechanics research."
---

[Link to Github repo](https://github.com/ashtencodes/tvtr_control/tree/rpi)

[Link to control software I wrote](https://github.com/ashtencodes/tvtr_control/tree/rpi/src/cr_control)

<img width="400px" class="rounded float-start pe-4 mx-auto" src="../img/rover/rover.png">

I built the software for a teleoperated rover for the purposes of terramechanics modeling research at the [RoSE Lab (Robotics Space Exploration Lab)](https://www.hsfl.hawaii.edu/planetary-surface-robots/) at UH Manoa. This rover's software was developed ROS (Robotics Operating System). The chassis was built by mechanical engineering students of the RoSE Lab

The main aspect of this project I worked on was the control software for the rover and a data collection pipeline to output data collected from the rover.

### Rover control software

I interfaced with the motors using a Roboclaw motor controller. I communicated with the motor controller with serial port programming, more specifically, the UART protocol. This is done in C/C++ through the linux serial port interface. I had trouble getting the Roboclaw libraries to work with this environment, so I instead decided to write it myself from scratch, although not every feature is implemented.

The following is the line of code that simply writes bytes to the UART serial port bus:

```cpp
int Roboclaw::WriteToEncoders(uint8_t* data, int nBytes) {
    int writeFlag = write(serialPort, data, nBytes);

    if (writeFlag != nBytes) return -1;

    return writeFlag;
}
```

It's quite simple to send out messages, but reading messages are a bit more complicated. You just need to set a timeout for when to give up on receiving messages back from the motor controller, although in c, there is a bit of a learning curve to interfacing with the linux serial port interface.

### Data collection pipeline

For the data collection pipeline, I took advantage of ROS features. This involves publishing data such as wheel speed, current, and IMU (inertial measurement unit) data to the ROS environment. I then used the rosbag record proces to subscribed to this published data and save it for data analysis at a later time.
