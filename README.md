<div align="center">

# 👋 Hi, I'm Aziz Marnissi

### ⚡ I put AI on silicon 🔬

🎓 Final-year Electrical Engineering @ **ENIT** &nbsp;·&nbsp; 📍 Tunis, Tunisia

💼 [LinkedIn](https://linkedin.com/in/aziz-marnissi) &nbsp;·&nbsp; 📧 [Email](mailto:aziz.marnissi@etudiant-enit.utm.tn)

</div>

> [!IMPORTANT]
> 🟢 **Open to a 4–6 month internship** in 🧠 Embedded AI, 🔌 FPGA or 🚀 AI hardware acceleration.

---

## 🧬 About

I connect algorithms to silicon so AI inference runs fast and lean, from FPGA kernels to microcontrollers.

- 🎯 **Focus:** hardware AI acceleration, Edge AI, robotics
- 🚁 **Building now:** deep-learning drone landing control (ROS2, PX4, Hailo-8L)
- 🎓 **Track:** SMART (Embedded Systems, Edge AI, FPGA, IoT)
- 🌍 **Languages:** 🇹🇳 Arabic (native) · 🇫🇷 French (fluent) · 🇬🇧 English (fluent) · 🇩🇪 German (A2)
- 🤝 **Activities:** CGE Club, IEEE Branch (2024–present)

## 📊 Speedups at a glance

🟪 FPGA (HLS) &nbsp; 🟨 Edge NPU &nbsp; 🟩 MCU &nbsp;·&nbsp; 1 block ≈ 5×

| Project | Speedup |
|---|---|
| 🧩 LeNet-5 CNN · PYNQ-Z2 | 🟪🟪🟪🟪🟪🟪🟪🟪🟪🟪🟪🟪🟪🟪🟪 **74×** |
| 🚁 UAV landing net · Hailo-8L NPU | 🟨🟨🟨🟨🟨🟨🟨🟨🟨🟨🟨🟨🟨 **65×** |
| 🌀 RoPE kernel | 🟪🟪🟪🟪🟪🟪🟪🟪🟪🟪 **49.9×** |
| 🔥 SiLU kernel | 🟪🟪🟪 **16.4×** |
| 🧮 MatMul kernel | 🟪🟪 **10×** |
| 📐 RMSNorm kernel | 🟪🟪 **9.9×** |
| 🎚️ Softmax kernel | 🟪🟪 **7.5×** |
| 💬 TinyGRU · ESP32 | 🟩 **3.6×** |
| 🎲 Greedy sampler | 🟪 **1.4×** |

```diff
- CPU              288 ms / MNIST image
+ FPGA (PYNQ-Z2)     3.9 ms / MNIST image   → 74×

- ESP32 baseline   251 ms / inference
+ ESP32 optimized    69 ms / inference      → 3.6×
```

## 🚀 Projects

<details open>
<summary><b>🧠 LLM kernels on FPGA</b> · WISECORP · 🟪 up to 49.9×</summary>

<br>

Feasibility study of which LLM primitives deserve hardware acceleration, using HLS kernels.

- ⚡ **49.9×** RoPE, **16.4×** SiLU, **10×** matmul vs. CPU
- 🔬 FP16 vs. INT4 trade-offs cut DSP/BRAM usage by up to **20% / 39%**
- 🛠️ `Vitis HLS` `Vivado` `Python`

</details>

<details>
<summary><b>⚡ LeNet-5 accelerator</b> · PYNQ-Z2 · 🟪 74×</summary>

<br>

CNN inference pipeline (2 conv + 3 fully-connected layers) split into 3 independent hardware blocks, quantized to INT8 (`ap_fixed`).

- 🏎️ 3.9 ms vs. 288 ms per MNIST image
- ✅ Validated via AXI-Lite register inspection and sentinel-value testing
- 🛠️ `Vitis HLS` `Vivado` `C/C++` `PYNQ-Z2`

</details>

<details>
<summary><b>🚁 Drone landing control</b> · UAV · 🟨 65×</summary>

<br>

Closed-loop HIL simulation pipeline to validate autonomous landing before flight.

- 📷 Raspberry Pi 5 + Hailo-8L NPU: **40 FPS at 25 ms**
- 🎯 **87.5% F1** after INT8 quantization
- 🛠️ `ROS2` `Gazebo` `PX4` `MAVLink` `QGroundControl` `OpenCV` `YOLOv8` `PID`

</details>

<details>
<summary><b>🛡️ SecureAI IDS</b> · TinyML intrusion detection for CAN bus · ESP32</summary>

<br>

Detects flooding, replay, spoofing and spike attacks with a pruned, quantized neural network.

- ✂️ Structural pruning: real reductions in size, RAM and latency
- 🔌 Validated on real ESP32 hardware via TensorFlow Lite Micro
- 🛠️ `Python` `TensorFlow` `TFLite Micro` `PlatformIO` `ESP32`

</details>

<details>
<summary><b>💬 TinyGRU-ESP32</b> · embedded text command controller · 🟩 3.6×</summary>

<br>

Bidirectional GRU intent-recognition model (81K params, **94.8% accuracy**) in PyTorch, deployed on ESP32 via quantized C inference (FP32 / INT8 / Hybrid) driving real GPIO actuators.

- ⏱️ 69 ms vs. 251 ms per inference
- 💾 **39% Flash savings** with INT8/Hybrid, no accuracy loss
- 🛠️ `PyTorch` `C` `PlatformIO` `ESP32`

</details>

<details>
<summary><b>🔧 RISC-V CPU</b> · Zybo FPGA · custom UART, PWM, I2C</summary>

<br>

RISC-V core with custom peripherals, validated on bare metal.

- 🛠️ `VHDL` `Vivado`

</details>

## 💼 Experience

- 🟣 **Jun–Jul 2026** · FPGA & AI Acceleration Intern, **WISECORP** (Tunis)
- 🟡 **Jun 2025** · Industrial Computing Intern, **SERGAZ** (Tunis): monitoring and diagnostics of three-phase motors and electrical cabinets for gas turbines
- 🔵 **2024 – present** · Engineering degree in Electrical Engineering, **ENIT**
- 🟢 **2022 – 2024** · Preparatory classes in Mathematics and Physics, **IPEIN**

## 🧰 Tech stack

| | Area | Tools |
|---|---|---|
| 🟣 | **Languages** | C/C++ · Python · VHDL |
| 🔴 | **EDA** | Vitis HLS · Vivado · Vitis · MATLAB |
| 🟡 | **Platforms** | PYNQ-Z2 · Zybo · Hailo NPU · Raspberry Pi 5 · BeagleBone Black · ESP32 · STM32 · Jetson Orin/Nano |
| 🟢 | **Machine learning** | TensorFlow · PyTorch · scikit-learn · OpenCV · CUDA · TensorRT |
| 🔵 | **Robotics** | ROS2 · Gazebo · PX4 · MAVLink · QGroundControl |

## 🏅 Certifications

- 📘 Supervised Learning with scikit-learn (DataCamp)
- 🔥 Deep Learning with PyTorch (DataCamp)
- 🌐 Intro to IoT (Cisco)

---

> [!TIP]
> 📬 Working on FPGA, Edge AI or robotics? Let's talk: [aziz.marnissi@etudiant-enit.utm.tn](mailto:aziz.marnissi@etudiant-enit.utm.tn)
