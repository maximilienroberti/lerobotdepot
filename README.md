![](media/lerobotdepot_logo.png)

Welcome to **LeRobotDepot**. This repository is listing open-source hardware, components, and 3D-printable projects compatible with the [LeRobot library](https://github.com/huggingface/lerobot). It helps users easily discover, build, and contribute to affordable, accessible robotics solutions powered by state-of-the-art AI.

## Table of Contents

- [Feetech Family](#feetech-family)
  - [Robot Arms](#robot-arms)
  - [Bi-manual Arms](#bi-manual-arms)
  - [Mobile Arms](#mobile-arms)
  - [Mobile Bi-manual Arms](#mobile-bi-manual-arms)
  - [Humanoid Robots](#humanoid-robots)
  - [Bipedal Robots](#bipedal-robots)
  - [Grippers & Accessories](#grippers--accessories)
  - [Track Axis](#track-axis)
- [Dynamixel Family](#dynamixel-family)
  - [Robot Arms](#robot-arms-dynamixel)
  - [Bi-manual Arms](#bi-manual-arms-dynamixel)
- [Common Accessories & Add-ons](#common-accessories--add-ons)
  - [Task Kits](#task-kits)
  - [Other Accessories](#other)
- [Teleoperation](#teleoperation)
- [Cameras](#cameras)
- [Contributing](#contributing)

---

# Feetech Family

Hardware in this family uses **Feetech motors**—primarily the STS3215 series (7.4V and 12V variants), plus a higher-torque drop-in option (STS3250). These motors are popular for their balance between performance and cost. *(Note: all listed servos share the same external dimensions.)*

- **[STS3215 (7.4V)](https://www.feetechrc.com/74v-19-kgcm-plastic-case-metal-tooth-magnetic-code-double-axis-ttl-series-steering-gear.html):** Typically offers a stall torque of approximately **16.5 kg·cm at 6V**. This option is often sufficient for basic robotics applications.  
  *Est. unit price:* **~$14 / ~€12 / ~¥96 (RMB)**

- **[STS3215 (12V)](https://www.feetechrc.com/12v-30kg-metal-shell-metal-tooth-iron-core-motor-magnetic-coding-double-shaft-ttl-series-steering-gear.html):** Delivers around **30 kg·cm** of stall torque, providing increased power for more demanding tasks.  
  *Est. unit price:* **~$16.5 / ~€14 / ~¥110 (RMB)**

- **[STS3250 (12V)](https://www.feetechrc.com/en/562636.html):** Same form factor, but delivers around **50 kg·cm** of stall torque for higher-load joints and heavier end-effectors.  
  *Est. unit price:* **~$55 / ~€46.5 / ~¥380 (RMB)**

> _Prices are rough single-unit estimates (excluding shipping/taxes) and may vary by reseller and region._

By standardizing on this Feetech form factor, projects in the Feetech Family maintain similar power and control characteristics, ensuring compatibility across accessories and modules.

## Robot Arms:

### [SO-100 & SO-101 Arms](https://github.com/TheRobotStudio/SO-ARM100)

This **5 DOF arm** is the recommended arm to get started with LeRobot—especially the 7.4V version.

<img src="media/so-arm100.jpg" width="500">

|             Price         | US    | EU    | RMB       |
|---------------------------|-------|-------|-----------|
| Follower and Leader arms  | $230  | €226  | ￥1343 |
| One Arm                   | $122  | €124  | ￥682  |

#### Accessories <a name="so-arm100-accessories"></a>

For detailed information on the various accessories available for the SO-ARM100, including mounting options and additional components, please refer to the [SO-ARM100 repository’s hardware documentation](https://github.com/TheRobotStudio/SO-ARM100?tab=readme-ov-file#hardware).

##### Wrist Cameras

The SO-ARM100 supports multiple wrist camera options to suit a variety of applications. There are three officially supported options and one community-developed alternative:

| Camera Name            |Reference Link                                                                                                 | Notes |
|------------------------|---------------------------------------------------------------------------------------------------------------|-------|
| [Vinmooog Webcam](https://amzn.eu/d/9nrIy5I)        |[SO-ARM100 Instructions](https://github.com/TheRobotStudio/SO-ARM100/tree/main/Optional/Wrist_Cam_Mount_Vinmooog_Webcam) | |
| 32x32mm UVC Module     |[SO-ARM100 Instructions](https://github.com/TheRobotStudio/SO-ARM100/tree/main/Optional/Wrist_Cam_Mount_32x32_UVC_Module)| |
| [Arducam 5MP Wide Angle](https://a.co/d/dFq7oRB) |[Le Kiwi STL File](https://github.com/SIGRobotics-UIUC/LeKiwi/blob/main/3DPrintMeshes/wrist_camera_mount.stl)| It can also be used with 32x32mm UVC modules, but if you don't use a wide-angle camera, the gripper will not appear in the camera view. |
| [RealSense™ D405](https://www.intelrealsense.com/depth-camera-d405/) |[SO-ARM100 Instructions](https://github.com/TheRobotStudio/SO-ARM100/tree/main/Optional/Wrist_Cam_Mount_RealSense_D405) | |
| [RealSense™ D435](https://www.intelrealsense.com/depth-camera-d435/)  | [SO-ARM100 Instructions](https://github.com/TheRobotStudio/SO-ARM100/tree/main/Optional/Wrist_Cam_Mount_RealSense_D435)                         | You can also use this mount with a Vinmooog camera using the included adapter. |


##### Haptic Sensors

- [WOWROBO Haptic sensor](https://shop.wowrobo.com/products/enhanced-anyskin-premium-crafted-editionwowskin)


##### Others
- [SO-ARM100 electronics mounting cover](https://grabcad.com/library/so100-arm-electronics-mounting-cover-and-stereo-cam-holder-1)
- [Magnetic Encoder Dummy Servo](https://github.com/avenhaus/SO-ARM100-Encoders)

#### Kits

You can find kits for the SO100 arms here:
- [partabot](https://partabot.com): Also include LeKiwi and [Aloha Mini](https://partabot.com/products/aloha-mini).
- [Seeed Studio](https://www.seeedstudio.com/Robot-Kit-c-2476.html): Also include LeKiwi.
- [WOWROBO](https://shop.wowrobo.com/collections/all): Also include Koch V1.1 and XLeRobot.
- [Phospho](https://robots.phospho.ai): Also include Open Duck Mini.
- [Autodiscovery](https://autodiscovery.eu/en/products/so-101-kit)

Both **assembled** and **non-assembled** kits are available, depending on the supplier.

---

### [jess-moss/moss-robot-arms](https://github.com/jess-moss/moss-robot-arms)
This **5 DOF arm** is similar to the SO-ARM100 but uses only the gripper as a 3D printed part. It is recommended to build or purchase the SO100 arm instead. While the Moss v1 robot is still supported, it will be deprecated. Additionally, 3D-printed parts for the SO-ARM100 are now available for purchase if you don't have a printer.

<img src="media/moss-robot-arm.png" width="500">

|        Price              | US    | EU    | RMB       |
|---------------------------|-------|-------|-----------|
| Follower and Leader arms  | $288  | €274  | ￥1631.46 |
| One Arm                   | $159  | €153  | ￥868.13  |

#### Accessories

See [SO-ARM100 Accessories](#so-arm100-accessories) for compatible components and mounts.

---

### [ajinkyagorad/SO-ARM107](https://github.com/ajinkyagorad/Lerobot-SO100-Arm/tree/777a90975373a8f5e9e56d468a24ab3dc5916ea4/hardware)

This is a **6 DOF arm**, based on the SO-ARM100 leader and follower arms, with an additional joint enabled by one more STS3215 servo motor.

<img src="media/so-arm107.jpg" width="500">

#### Price

The price is roughly equivalent to the SO-ARM100, plus the cost of one extra Feetech servo motor—either 7.4V or 12V, depending on your chosen configuration.

#### Accessories

For wrist cameras, haptic sensors, and other modules, see [SO-ARM100 Accessories](#so-arm100-accessories) for compatible components.

---

### SAM arm

This is a **6 DOF arm**, developed by the community around the [SimpleAutomation repository](https://github.com/SimpleAutomationOrg/SimpleAutomation). It is a refined version of the SO-ARM100, offering enhanced movement precision and a gripper better optimized for handling small objects.

<img src="media/SAM_arm.png" width="500">

- [Discord Channel](https://t.co/pPVt7dVbnJ)
- [Discord message on Bill Of Materials](https://discord.com/channels/1306427593586901092/1308906584239243274/1324588976312684595)
- [Discord message on Beta v1.1 STEP files](https://discord.com/channels/1306427593586901092/1308906584239243274/1336551154368253972)


|        Price              | US    |
|---------------------------|-------|
| Follower and Leader arms  | ± $450|


---

## Bi-manual Arms

### [Mr-C4T/AB-SO-BOT](https://github.com/Mr-C4T/AB-SO-BOT)

AB-SO-BOT is built using a combination of 3D-printed parts and standard 4040 T-slot aluminium extrusions to create a customizable and modular body for the SO-ARM100.

<img src="media/ab-so-bot.png" width="500">

---

## Mobile Arms

### [SIGRobotics-UIUC/LeKiwi](https://github.com/SIGRobotics-UIUC/LeKiwi)
Mobile version of the SO-ARM100.

<img src="media/LeKiwi.png" width="500">


| Price              | US      | EU      |
|--------------------|---------|---------|
| 12V                | $488.21 | €542.56 |
| 5V                 | $524.95 | €525.9  |
| Base only (5V)     | $251.95 | €306.9  |
| Base only (12V)    | $257.43 | €305    |
| Base only wired    | $174    | €233.3  |

---

## Mobile Bi-manual Arms

### [Vector-Wangel/XLeRobot](https://github.com/Vector-Wangel/XLeRobot)

Practical low-cost **dual-arm mobile home robot**, built on top of the LeKiwi base and SO101 arms.

<img src="media/xlerobot.png" width="500">

| Price (buy parts yourself)                | US     | EU     | RMB        |
|------------------------------------------|--------|--------|------------|
| Basic (use your laptop, single RGB cam)  | ~$660  | ~€680  | ~¥3999     |

#### Kits

- Developer assembly kit available via WOWROBO.
- See the project documentation for the latest kit details: https://xlerobot.readthedocs.io/

### [timqian/bambot](https://github.com/timqian/bambot)

Mobile version of the SO-ARM100 with two arms.

<img alt="Bambot, open source, low-cost humanoid ($300)" src="media/bambot.png" width="500">

|              Price        | US     | EU     | RMB       |
|---------------------------|--------|--------|-----------|
| Total                     | ~ $300 | ~ €300 | ~ ￥2000 |

---

## Bipedal Robots

### [apirrone/Open_Duck_Mini](https://github.com/apirrone/Open_Duck_Mini)

Miniature version of the BDX Droid by Disney.

<img src="media/open_duck_mini.png" width="500">

#### Price

~€410

---

## Humanoid Robots

### [TheRobotStudio/HOPEJr](https://github.com/TheRobotStudio/HOPEJr)
A project for a full body robot—currently featuring the torso and arms.

<img src="media/hopejr.png" width="500">

---

## Grippers & Accessories

### [pollen-robotics/PincOpen](https://github.com/pollen-robotics/PincOpen)

Parallel-finger gripper compatible with SO-ARM100.

<img src="media/PincOpen.png" width="500">

#### Price:
~€25

---

### [Chojins/LeRobot-S0-100-Models](https://github.com/Chojins/LeRobot-S0-100-Models)

Precise gripper compatible with SO-ARM100.

<img src="media/so-100_chojins_gripper.png" width="500">

---

## Track axis

### [avenhaus/SO-ARM100-Track-Axis](https://github.com/avenhaus/SO-ARM100-Track-Axis)

It provides an additional axis to the SO-ARM100 robot arm.

<img src="media/track_axis.png" width="500">

---
# Dynamixel Family

Hardware in this family uses Dynamixel servo motors, which are considered more of an industry standard than Feetech motors.

## Robot Arms: <a name="robot-arms-dynamixel"></a>

### [jess-moss/koch-v1-1](https://github.com/jess-moss/koch-v1-1)

The Koch-v1-1 is a 5 DOF robotic arm. If you want to familiarise yourself with more industry standard Dynamixel servo motors, this project could be a good starting point. Compared to the SO-ARM100, you will have less torque and a more limited range of movement from its base.

<img src="media/koch-v1-1.png" width="500">


|         Price           | US    | EU    | UK    | RMB   | JPY    |
|-------------------------|-------|-------|-------|-------|--------|
| Follower and Leader arms| $477  | €673  | £507  | ¥3947 | ¥22439 |
| Leader Arm              | $278  | €368  | £285  | ¥2251 | ¥15446 |
| Follower Arm            | $199  | €305  | £222  | ¥1696 | ¥6993  |

#### Accessories

##### Wrist Cameras

The Koch-v1-1 supports 2 wrist camera options:

| Camera Name | Reference Link | Notes |
|-------------|----------------|-------|
| [SVPRO 1080P](https://a.co/d/bbgtN1L)| [Discord Message with STL file](https://discord.com/channels/1216765309076115607/1243077809828790363/1311493401157304350) | |
| N/A | [WOWROBO Gripper-Camera Kit](https://shop.wowrobo.com/products/gripper-camera-kit-for-koch-v1-1) | Kit including the gripper, the camera mount and the camera |

##### Haptic Sensors

- [WOWROBO Haptic sensor](https://shop.wowrobo.com/products/enhanced-anyskin-premium-crafted-editionwowskin)

#### Kits

- Robotic arm inspired by Kochv-1-1: [WOWROBO Twinarm](https://shop.wowrobo.com/products/wowrobo-twinarm-robotic-arm-set-inspired-by-koch-v1-1)

---

## Bi-manual Arms: <a name="bi-manual-arms-dynamixel"></a>

### [ALOHA 2](https://aloha-2.github.io)


ALOHA 2 is a bimanual teleoperation system that uses two types of arms—a pair of smaller, ergonomically designed leader arms and two robust follower arms—to support coordinated dual-arm manipulation. Each arm offers **6 degrees of freedom (6 DOF)**, which provides an extensive range of motion for accessing various positions and orientations.

The system is designed for research in fine-grained bimanual manipulation. Its construction includes enhanced gripper mechanisms, a passive gravity compensation system, and a rigid frame that supports precise and repeatable operations for complex tasks. These advanced features and components are reflected in its higher cost compared to more basic robotic arm solutions.

<img src="media/aloha-2.png" width="500">

#### Price

~$27,000

#### Kits

- [Aloha Stationary](https://www.trossenrobotics.com/aloha-stationary) by [Trossen Robotics](https://www.trossenrobotics.com)

---

# Common Accessories & Add-ons

## Task kits

### [cgreer/robot-task-kit](https://github.com/cgreer/robot-task-kit)

- "T" for push T task.
- A "toaster" with 2 pieces of "toast".
- A paper towel base & rod + paper towel roll.
- Cube.
- Ring.

<img src="media/task_kit.png" width="500">

---

### [Hugging Face rectangular prism](https://github.com/jess-moss/koch-v1-1/tree/main/hardware/extras/STL)

<img src="media/huggingface_rectangular_prism.jpg" width="500">

---

## Other

### [Self-Fusing Silicone Rubber](https://www.3m.com/3M/en_US/p/d/b00011950/)
To increase friction on gripper.
  
  <img src="media/silicone_rubber.png" width="500">

### [Foam Tape](https://www.amazon.com/s?k=Window%2BFoam%2BSeal%2BTape%2B1%2F2Inch%2BWide%2BX%2B1%2F2Inch)
Alternative to silicone rubber for increasing friction. You can add screws to avoid losing the foam tips. 

  <img src="media/foam_tape.jpg" width="500">
  
---

# Teleoperation

## [max-titov/finger-tracker](https://github.com/max-titov/finger-tracker)

Hardware that attaches to the back of your hand and fingertips that tracks 16 degrees of freedom. Compatible with [HOPEJr hands](#therobotstudiohopejr).


<img src="media/finger_tracker.png" width="500">


---

# Cameras


| Name                     | Price Range      | Link | Resolution | FPS  | Wide Angle                                   | Microphone |
|--------------------------|------------------|------|------------|------|----------------------------------------------|------------|
| Innomaker 1080P USB2.0    | ± $18, €16       | [Innomaker Link](https://www.inno-maker.com/product-category/products/uvc-cameras/low-cost/) | 1920×1080  | 30   | Fov(D) = 130° <br> Fov(H) = 103°              | No         |
| Innomaker 720p USB2.0     | ± $10, €14       | [Innomaker Link](https://www.inno-maker.com/product-category/products/uvc-cameras/low-cost/) | 1280×720   | 30   | FOV (D) = 120° <br> FOV (H) = 102°             | No         |
| Innomaker OV9281 USB 2.0  | ± $36, €42       | [Innomaker Link](https://www.inno-maker.com/product/u20cam-9281m/) | 1280×800   | 120  | FOV Up to 148°                               | No         |
| Vinmooog Webcam          | ± $14, €12       | [Amazon Link](https://www.amazon.nl/-/en/Microphone-Adjustable-Conference-Streaming-Compatible/dp/B0BG1YJWFN/) | 1920×1080  | N/A  | N/A                                          | Yes        |

## Others
- https://www.amazon.co.uk/ELP-Conferencing-Fisheye-0-01Lux-Computer/dp/B08Y1KY5T9?th=1
- https://www.amazon.com/dp/B07CSJN2KH

---

# Contributing

Interested in contributing? Please take a moment to review our [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to get started.

