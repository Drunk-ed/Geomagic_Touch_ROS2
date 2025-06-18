# Geomagic_Touch_ROS2

**ROS 2 Port of the Geomagic Touch Driver with Interbotix RX200 Teleoperation Support**

---

## Overview

This repository contains a ROS 2 port of the [Geomagic Touch ROS driver](https://github.com/bharatm11/Geomagic_Touch_ROS_Drivers) originally developed by **[@bharatm11](https://github.com/bharatm11)** and later integrated for RX200 teleoperation by **[@KaranK369](https://github.com/KaranK369)** in his [rx200_teleoperation repo](https://github.com/KaranK369/rx200_teleoperation/tree/main/Geomagic_Touch_ROS/src).

This version brings the driver and teleoperation functionality to **ROS 2 (Humble)**, enabling real-time control of the **Interbotix RX200** robot arm using the **Geomagic Touch Haptic Device**.

---

## Installation

### 1. Install Geomagic Touch Drivers

Install the **Touch Device Driver** and **OpenHaptics SDK** (Linux):

📦 [OpenHaptics Developer Edition v3.4 – Ubuntu 20.04](https://support.3dsystems.com/s/article/OpenHaptics-for-Linux-Developer-Edition-v34?language=en_US)

> After installing, reboot your system to ensure the device is detected properly.

---

## ROS 2 Workspace Setup

1. Clone this repo into your ROS 2 workspace:

```bash
cd ~/your_ros2_ws/src
git clone https://github.com/Drunk-ed/phantom_to_interbotix_teleop.git
cd ..
colcon build
source install/setup.bash
