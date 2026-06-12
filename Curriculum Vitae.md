# Ethan Yi-Chien Chiang (江易謙)

- Taichung, Taiwan
- Phone: +886956236659
- Email: <ethannt1000@gmail.com>
- LinkedIn: <https://www.linkedin.com/in/yi-chien-chiang-8b32032a4>
- GitHub: <https://github.com/EthanNT1000>

---

## Professional Summary

Embedded systems engineer with 5 years of experience spanning aerospace firmware, instrumentation, and autonomous vehicles. Specializes in the intersection of low-level firmware (C/C++, STM32, FreeRTOS) and robotics autonomy — developing Ardupilot-based USVs, building Gazebo simulation platforms, and applying reinforcement learning (TD3) to automate control-parameter tuning. Proven record shipping mission-critical, high-reliability systems for rocket subsystems and precision instruments. Open to relocation and visa sponsorship.

---

## Work Experience

### Firmware Engineer

**Taiwan Innovative Space Inc., Taipei, Taiwan** — May 2023 – Present

- Rescued a stalled safety-critical ground-station firmware project (STM32F746) and delivered it within a one-month deadline: sub-GHz RF command link (AT86RF215), encrypted command framing, two-unit RTC/UDP time synchronization, and a hardware-interlocked ARM→DESTRUCT state machine.
- Took over the dual-core (Cortex-M7/M4) STM32H7 flight software after the original developer's departure: implemented inter-core navigation-data sharing via SRAM4 shared memory and hardware semaphores, redundant flight-termination command dispatch, and a headless dual-core build/flash toolchain.
- Resolved a critical data-loss defect in a CAN-to-UART flight sensor controller by moving sample packing into the CAN ISR with a zero-alloc circular buffer and a zero-copy DMA UART path; verified zero packet loss across a 6.4 kHz accelerometer stream (4 × 1.6 kHz) using per-packet sequence numbers and a custom InfluxDB validation tool.
- Extended a cross-platform C++ firmware layer (libopencm3-based) across STM32 F1/F4/F7 with multiple new drivers — a calibrated microsecond timer, a zero-copy DMA UART, interrupt-driven I2C with STM32F1 bus-reset recovery, and a DPS310 pressure-sensor driver — and performed STM32H7 register-level bring-up (FDCAN, I2C) in the open-source HAL fork.
- Developing the autopilot for an ArduPilot-based unmanned surface vehicle (USV): sensor calibration and a custom Lua servo-failsafe extending ArduPilot's native behavior, with control parameters auto-tuned by a TD3 reinforcement-learning pipeline in Gazebo simulation.

### Software Engineer

**Good Will Instrument Co., Ltd., Taipei, Taiwan** — September 2021 – March 2023

- Developed the user interface for digital storage oscilloscopes using WPF with MVVM architecture.
- Implemented software-based protocol decoding and analysis for CAN, LIN, I2C, SPI, and UART to support signal visualization and debugging.

### Mechatronics Engineer

**Huro Auto Co., Ltd., Taipei, Taiwan** — March 2021 – September 2021

- Built and maintained mechatronics systems for electric buses, focusing on CAN Bus network integration to ensure reliable communication between control units.
- Conducted diagnostic testing and troubleshooting of CAN Bus systems.

### Professional Development & National Service

**Taiwan** — September 2019 – February 2021

- Completed compulsory military service (Sep 2019 – Jan 2020).
- Self-studied English and earned a TOEFL iBT score of 86 (ETS, September 2020).
- Completed an electric-vehicle mechatronics training course, building the CAN Bus and EV powertrain foundation applied directly in the subsequent Mechatronics Engineer role.

---

## Projects

- [**Gazebo USV Simulation Platform**](https://github.com/EthanNT1000/asv_wave_sim/tree/ament_environment_hooks) (2025): Forked the open-source ASV wave simulation, enhanced hydrodynamic physics and runtime performance, and extended it into a full Gazebo-based USV simulation environment for hardware-free testing.
- [**GStreamer UAV Video Link**](https://github.com/EthanNT1000/gst-uav-videolink) (2026): Built a UAV video-link pipeline in C/GStreamer — camera → H.264/H.265 encode → RTP/RTSP → decode/display — with configurable encode presets, live FPS monitoring, and MAVLink VIDEO_STREAM_INFORMATION for QGroundControl auto-discovery; characterized software encoding CPU cost and latency across presets on ARM Cortex-A76 (H.264 ultrafast: ~10% CPU / 7 ms; H.265 ultrafast: ~100% CPU / 144 ms encode latency — motivating hardware encoder selection on Jetson/i.MX targets).
- [**Pico C++ Firmware Template**](https://github.com/EthanNT1000/pico-cpp-template.git) (2025): Developed a general-purpose RP2040 firmware template integrating FreeRTOS, micro-ROS, and an MCP2515 CAN Bus driver with a task-based architecture for rapid embedded project setup.

---

## Education

### Bachelor of Science in Automation Engineering

**National Formosa University, Yunlin County, Taiwan** — September 2015 – June 2019

### Vocational High School Diploma in Control Engineering

**Taichung Industrial High School, Taichung City, Taiwan** — September 2012 – July 2015

---

## Certifications

- TOEFL iBT: Score of 86, Educational Testing Service (ETS), September 13, 2020

---

## Skills

- **Programming**: C/C++, C#, Python
- **Frameworks**: WPF (MVVM), STM32, FreeRTOS, libopencm3, Ardupilot, ROS2, micro-ROS, LwIP
- **Hardware**: RP2040 (Raspberry Pi Pico), MCP2515 CAN controller
- **Protocols**: CAN Bus, LIN Bus, I2C, SPI, UART, MAVLink
- **Simulation**: Gazebo, Ardupilot SITL, ASV Wave Simulation
- **ML / Robotics**: TD3 (Reinforcement Learning), Autonomous Vehicle Parameter Tuning
- **Tools**: Git, Visual Studio, STM32CubeIDE, OpenOCD, Lua scripting
