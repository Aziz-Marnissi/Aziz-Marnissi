# Hi, I'm Aziz Marnissi

**I put AI on silicon.**

Final-year electrical engineering student at ENIT (Tunis), SMART track: Embedded Systems, Edge AI, FPGA, IoT. I connect algorithms to silicon so AI inference runs fast and lean, from FPGA kernels to microcontrollers.

**Open to a 4–6 month internship** in Embedded AI, FPGA or AI hardware acceleration.

[LinkedIn](https://linkedin.com/in/aziz-marnissi) · [Email](mailto:aziz.marnissi@etudiant-enit.utm.tn) · Tunis, Tunisia

---

## About

- Focus: hardware AI acceleration, Edge AI, robotics
- Currently building: deep-learning drone landing control (ROS2, PX4, Hailo-8L)
- Languages: Arabic (native), French (fluent), English (fluent), German (A2)
- Activities: CGE Club, IEEE Branch (2024–present)

## Measured speedups

| Project | Platform | Speedup |
|---|---|---|
| LeNet-5 CNN | PYNQ-Z2 (Vitis HLS) | 74× vs. CPU |
| UAV landing network | Raspberry Pi 5 + Hailo-8L NPU | 65× vs. CPU |
| RoPE kernel | FPGA (Vitis HLS) | 49.9× vs. CPU |
| SiLU kernel | FPGA (Vitis HLS) | 16.4× vs. CPU |
| MatMul kernel | FPGA (Vitis HLS) | 10× vs. CPU |
| RMSNorm kernel | FPGA (Vitis HLS) | 9.9× vs. CPU |
| Softmax kernel | FPGA (Vitis HLS) | 7.5× vs. CPU |
| TinyGRU | ESP32 (INT8/Hybrid) | 3.6× |
| Greedy sampler | FPGA (Vitis HLS) | 1.4× vs. CPU |

## Projects

### LLM kernels on FPGA (WISECORP)
Feasibility study of which LLM primitives deserve hardware acceleration, using HLS kernels. Up to 49.9× (RoPE), 16.4× (SiLU) and 10× (matmul) vs. CPU. FP16 vs. INT4 trade-offs reduced DSP/BRAM usage by up to 20% / 39%.
`Vitis HLS` `Vivado` `Python`

### Hardware CNN accelerator (LeNet-5) on FPGA
CNN inference pipeline (2 conv + 3 fully-connected layers) split into 3 independent hardware blocks, quantized to INT8 (`ap_fixed`). 74× compute speedup vs. CPU (3.9 ms vs. 288 ms per MNIST image), validated via AXI-Lite register inspection and sentinel-value testing.
`Vitis HLS` `Vivado` `C/C++` `PYNQ-Z2`

### Deep learning-based drone landing control (UAV)
Closed-loop HIL simulation pipeline to validate autonomous landing before flight. Deployed on Raspberry Pi 5 with Hailo-8L NPU: 40 FPS at 25 ms (65× vs. CPU), 87.5% F1 after INT8 quantization.
`ROS2` `Gazebo` `PX4` `MAVLink` `QGroundControl` `OpenCV` `YOLOv8` `PID`

### SecureAI IDS: TinyML intrusion detection for CAN bus
Embedded AI system detecting flooding, replay, spoofing and spike attacks with a pruned, quantized neural network. Structural pruning gives real reductions in size, RAM and latency. Validated on real ESP32 hardware via TensorFlow Lite Micro.
`Python` `TensorFlow` `TFLite Micro` `PlatformIO` `ESP32`

### TinyGRU-ESP32: embedded text command controller
Bidirectional GRU intent-recognition model (81K params, 94.8% accuracy) in PyTorch, deployed on ESP32 via quantized C inference (FP32 / INT8 / Hybrid) driving real GPIO actuators. 3.6× faster inference (69 ms vs. 251 ms) and 39% Flash savings with no accuracy loss.
`PyTorch` `C` `PlatformIO` `ESP32`

### RISC-V CPU with custom peripherals
RISC-V core on a Zybo FPGA with custom UART, PWM and I2C, validated on bare metal.
`VHDL` `Vivado`

## Experience

| When | Role |
|---|---|
| Jun–Jul 2026 | **FPGA & AI Acceleration Intern**, WISECORP, Tunis |
| Jun 2025 | **Industrial Computing Intern**, SERGAZ, Tunis: monitoring and diagnostics of three-phase motors and electrical cabinets for gas turbines |
| 2024 – present | **Engineering degree in Electrical Engineering**, ENIT, SMART track |
| 2022 – 2024 | **Preparatory classes** (Mathematics and Physics), IPEIN |

## Tech stack

| Area | Tools |
|---|---|
| Languages | C/C++, Python, VHDL |
| EDA | Vitis HLS, Vivado, Vitis, MATLAB |
| Platforms | PYNQ-Z2, Zybo, Hailo NPU, Raspberry Pi 5, BeagleBone Black, ESP32, STM32, Jetson Orin/Nano |
| Machine learning | TensorFlow, PyTorch, scikit-learn, OpenCV, CUDA, TensorRT |
| Robotics | ROS2, Gazebo, PX4, MAVLink, QGroundControl |

## Certifications

- Supervised Learning with scikit-learn (DataCamp)
- Deep Learning with PyTorch (DataCamp)
- Intro to IoT (Cisco)
