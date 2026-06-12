# Yi-Chien Chiang (江易謙)

Firmware & Robotics Engineer based in Taiwan. I build embedded systems for aerospace applications and autonomous surface vehicles.

## What I'm working on

- Deploying and tuning an **Ardupilot USV** — parameter configuration, sensor calibration, and custom Lua-based servo failsafe
- **Gazebo USV simulation platform** built on an enhanced fork of the ASV wave simulator
- **TD3 reinforcement learning pipeline** for automated Ardupilot parameter tuning, trained against the Gazebo sim

## Tech

**Languages:** C/C++, C#, Python  
**Embedded:** STM32, FreeRTOS, Ardupilot, MAVLink  
**Protocols:** CAN Bus, I2C, SPI, UART  
**Simulation:** Gazebo, Ardupilot SITL  
**Other:** WPF/MVVM, ROS2, Lua

## Repos

- [**Gazebo USV Simulation Platform**](https://github.com/EthanNT1000/asv_wave_sim/tree/ament_environment_hooks) (2025): Forked the open-source ASV wave simulation, enhanced hydrodynamic physics and runtime performance, and extended it into a full Gazebo-based USV simulation environment for hardware-free testing.
- [**GStreamer UAV Video Link**](https://github.com/EthanNT1000/gst-uav-videolink) (2026): Built a UAV video-link pipeline in C/GStreamer — camera → H.264/H.265 encode → RTP/RTSP → decode/display — with configurable encode presets, live FPS monitoring, and MAVLink VIDEO_STREAM_INFORMATION for QGroundControl auto-discovery; characterized software encoding CPU cost and latency across presets on ARM Cortex-A76 (H.264 ultrafast: ~10% CPU / 7 ms; H.265 ultrafast: ~100% CPU / 144 ms encode latency — motivating hardware encoder selection on Jetson/i.MX targets).
- [**Pico C++ Firmware Template**](https://github.com/EthanNT1000/pico-cpp-template.git) (2025): Developed a general-purpose RP2040 firmware template integrating FreeRTOS, micro-ROS, and an MCP2515 CAN Bus driver with a task-based architecture for rapid embedded project setup.

## Links

- [LinkedIn](https://www.linkedin.com/in/yi-chien-chiang-8b32032a4)
- [Curriculum Vitae](./Curriculum%20Vitae.md)
- Email: ethannt1000@gmail.com
