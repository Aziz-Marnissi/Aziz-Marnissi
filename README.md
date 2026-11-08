<div align="center">

<img src="assets/hero.svg" alt="Aziz Marnissi. I put AI on silicon." width="100%"/>

<br/>

<a href="https://linkedin.com/in/aziz-marnissi"><img src="https://img.shields.io/badge/LinkedIn-aziz--marnissi-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:aziz.marnissi@etudiant-enit.utm.tn"><img src="https://img.shields.io/badge/Email-Get_in_touch-8b5cf6?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="assets/Aziz_Marnissi_CV.pdf"><img src="https://img.shields.io/badge/Download-CV-fbbf24?style=for-the-badge&logo=readthedocs&logoColor=black" alt="Download CV"/></a>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=2600&pause=900&color=A78BFA&center=true&vCenter=true&width=760&height=40&lines=HLS+kernels+on+FPGA+%E2%86%92+49.9%C3%97+faster+RoPE;74%C3%97+CNN+speedup+on+PYNQ-Z2;INT8+models+on+ESP32+and+Hailo+NPU;Open+to+a+4%E2%80%936+month+internship" alt="Typing animation"/>

</div>

<img src="assets/divider.svg" width="100%" alt=""/>

## About

```python
class Aziz:
    school      = "ENIT · Electrical Engineering · SMART track (Embedded, Edge AI, FPGA, IoT)"
    focus       = ["Hardware AI acceleration", "Edge AI", "Robotics"]
    building    = "Deep-learning drone landing control: ROS2, PX4, Hailo-8L"
    languages   = {"Arabic": "native", "French": "fluent", "English": "fluent", "German": "A2"}
    looking_for = "4–6 month internship in Embedded AI, FPGA or AI hardware acceleration"
```

I bridge algorithms and silicon so AI inference runs fast and lean: HLS kernels on FPGA, quantized models on microcontrollers, and NPU deployment on real robots.

## Speedups

<img src="assets/speedups.svg" width="100%" alt="Measured speedups: 74x LeNet-5 on FPGA, 65x UAV net on Hailo NPU, 49.9x RoPE, 16.4x SiLU"/>

<img src="assets/divider.svg" width="100%" alt=""/>

## Projects

<table>
<tr>
<td width="50%" valign="top">

### 🧠 LLM kernels on FPGA
<sub>WISECORP · Vitis HLS · Vivado</sub>

Feasibility study of which LLM primitives deserve hardware acceleration. **49.9× RoPE**, **16.4× SiLU**, **10× matmul** vs. CPU. FP16 vs. INT4 trade-offs cut DSP/BRAM usage by up to **20% / 39%**.

<a href="https://github.com/Aziz-Marnissi?tab=repositories"><img src="https://img.shields.io/badge/Code-view-8b5cf6?style=flat-square" alt=""/></a>

</td>
<td width="50%" valign="top">

### ⚡ LeNet-5 accelerator
<sub>PYNQ-Z2 · Vitis HLS · INT8 `ap_fixed`</sub>

CNN inference pipeline split into 3 independent hardware blocks. **74× faster** than CPU (3.9 ms vs. 288 ms per MNIST image), validated via AXI-Lite register inspection.

<a href="https://github.com/Aziz-Marnissi?tab=repositories"><img src="https://img.shields.io/badge/Code-view-8b5cf6?style=flat-square" alt=""/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🚁 Drone landing control
<sub>ROS2 · Gazebo · PX4 · Raspberry Pi 5 · Hailo-8L</sub>

Closed-loop HIL pipeline to validate autonomous landing before flight. Runs at **40 FPS (25 ms)**, **65× vs. CPU**, with **87.5% F1** after INT8 quantization.

<a href="https://github.com/Aziz-Marnissi?tab=repositories"><img src="https://img.shields.io/badge/Code-view-8b5cf6?style=flat-square" alt=""/></a>

</td>
<td width="50%" valign="top">

### 🛡️ SecureAI IDS
<sub>ESP32 · TFLite Micro · CAN bus</sub>

TinyML intrusion detection for flooding, replay, spoofing and spike attacks. Structural pruning gives real size, RAM and latency gains, validated on hardware.

<a href="https://github.com/Aziz-Marnissi?tab=repositories"><img src="https://img.shields.io/badge/Code-view-8b5cf6?style=flat-square" alt=""/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 💬 TinyGRU-ESP32
<sub>PyTorch · quantized C · GPIO</sub>

Bidirectional GRU intent model (81K params, **94.8% accuracy**) driving real actuators. INT8/Hybrid gives **3.6× faster** inference and **39% less Flash** with no accuracy loss.

<a href="https://github.com/Aziz-Marnissi?tab=repositories"><img src="https://img.shields.io/badge/Code-view-8b5cf6?style=flat-square" alt=""/></a>

</td>
<td width="50%" valign="top">

### 🔧 RISC-V CPU
<sub>Zybo FPGA · VHDL</sub>

RISC-V core with custom UART, PWM and I2C peripherals, validated on bare metal.

<a href="https://github.com/Aziz-Marnissi?tab=repositories"><img src="https://img.shields.io/badge/Code-view-8b5cf6?style=flat-square" alt=""/></a>

</td>
</tr>
</table>

## Experience

| When | Where | What |
|---|---|---|
| Jun–Jul 2026 | **WISECORP** · FPGA & AI Acceleration Intern | HLS feasibility study for LLM primitives on FPGA |
| Jun 2025 | **SERGAZ** · Industrial Computing Intern | Vibration/temperature monitoring and diagnostics for gas-turbine motors and cabinets |
| 2024 – now | **ENIT** · Electrical Engineering, SMART track | Embedded systems, Edge AI, FPGA, IoT |
| 2022 – 2024 | **IPEIN** · Preparatory classes | Mathematics and Physics |

## Stack

<table>
<tr><td><b>Languages</b></td><td>
<img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black"/>
<img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/VHDL-6d4fd8?style=flat-square"/>
<img src="https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white"/>
</td></tr>
<tr><td><b>FPGA & EDA</b></td><td>
<img src="https://img.shields.io/badge/Vitis_HLS-ED1C24?style=flat-square&logo=amd&logoColor=white"/>
<img src="https://img.shields.io/badge/Vivado-ED1C24?style=flat-square&logo=amd&logoColor=white"/>
<img src="https://img.shields.io/badge/PYNQ--Z2-f59e0b?style=flat-square"/>
<img src="https://img.shields.io/badge/Zybo-f59e0b?style=flat-square"/>
</td></tr>
<tr><td><b>Edge hardware</b></td><td>
<img src="https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white"/>
<img src="https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white"/>
<img src="https://img.shields.io/badge/Raspberry_Pi_5-A22846?style=flat-square&logo=raspberrypi&logoColor=white"/>
<img src="https://img.shields.io/badge/Hailo--8L-8b5cf6?style=flat-square"/>
<img src="https://img.shields.io/badge/Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white"/>
<img src="https://img.shields.io/badge/BeagleBone-f59e0b?style=flat-square"/>
</td></tr>
<tr><td><b>Machine learning</b></td><td>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/TFLite_Micro-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/TensorRT-76B900?style=flat-square&logo=nvidia&logoColor=white"/>
<img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white"/>
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white"/>
</td></tr>
<tr><td><b>Robotics</b></td><td>
<img src="https://img.shields.io/badge/ROS2-22314E?style=flat-square&logo=ros&logoColor=white"/>
<img src="https://img.shields.io/badge/Gazebo-FF9900?style=flat-square"/>
<img src="https://img.shields.io/badge/PX4-3f51b5?style=flat-square"/>
<img src="https://img.shields.io/badge/MAVLink-0288d1?style=flat-square"/>
<img src="https://img.shields.io/badge/QGroundControl-0d47a1?style=flat-square"/>
</td></tr>
</table>

## GitHub stats

<div align="center">
<img height="170" src="https://github-readme-stats.vercel.app/api?username=Aziz-Marnissi&show_icons=true&hide_border=true&bg_color=07060d&title_color=a78bfa&icon_color=fbbf24&text_color=c9c5e0&ring_color=a78bfa&border_radius=12" alt="GitHub stats"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Aziz-Marnissi&layout=compact&hide_border=true&bg_color=07060d&title_color=a78bfa&text_color=c9c5e0&border_radius=12" alt="Top languages"/>
</div>

<img src="assets/divider.svg" width="100%" alt=""/>

<div align="center">

**Open to a 4–6 month internship** · Embedded AI · FPGA · AI hardware acceleration

<a href="mailto:aziz.marnissi@etudiant-enit.utm.tn">aziz.marnissi@etudiant-enit.utm.tn</a> · Tunis, Tunisia

</div>
