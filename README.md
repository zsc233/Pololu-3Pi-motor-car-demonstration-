# Pololu-3Pi-motor-car-demonstration-
This is a reposity only for demostration.

Public demo of a Pololu 3Pi+ (ATmega32U4) autonomous robot : closed-loop motion (PID), waypoint navigation, IR surface reflectance sensors, and magnetic puck detection with an FSM.  
基于 Pololu 3Pi+（ATmega32U4）的自主小车演示：PID 闭环运动、路径点导航、红外传感器、磁性目标探测，有限状态机（FSM）。

## Demo
<video src="assets/Pololu-3Pi-motor-car-demonstration.mp4" controls loop muted playsinline style="max-width: 100%;"></video>
![demo](assets/Pololu-3Pi-motor-car-demonstration.mp4)
https://youtube.com/shorts/7LqzaG9Dz_I

## Modules 模块
- **Hardware**：Pololu 3Pi+ 32U4（编码器Encoder、5×线传感器** IR surface reflectance sensors**、LIS3MDL 磁力计magnetometer）
- **Firmware**：Arduino C/C++
- **Core headers**：
  - `Motors.h` — 电机方向/PWM 与安全限幅  
  - `PID.h` — 离散 PID，简单防积分饱和  
  - `Encoders.h` — 正交编码器 ISR 解码  
  - `Kinematics.h` — 里程计/运动学（mm/计数、轮距/轮半径）  
  - `LineSensors.h` — ADC 读取、校准与归一化  
  - `Magnetometer.h` — 磁力探测 
  - `lcd.h` / `oled.h` — 屏幕显示

## 源码访问（私有）Source Code Access (Private)
The source code is hosted in a **private** repo: 本项目源码为: “ https://github.com/zsc233/motor-car-control.git ” 。如需访问请：
>在本仓库提交 Issue（标题：申请源码访问，用途说明），Submit an issue in this repository (title: Request access to source code, include your intended use)**或OR**
>Email 发送邮件至 zsc_233@outlook.com，附上您的GitHub 用户名与用途说明with your GitHub username and a brief description of your intended use.。
>**Terms**:将视情况临时授予只读权限。 read-only, no re-distribution.


  
