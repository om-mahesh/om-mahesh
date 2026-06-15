<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,100:1F6FEB&height=200&section=header&text=Om%20Maheshwari&fontColor=58A6FF&fontSize=50&animation=fadeIn&fontAlignY=35&desc=Hardware%20Engineer%20%7C%20VLSI%20Researcher%20%7C%20RISC-V&descAlignY=58&descSize=18" />

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=650&lines=Lossless+RISC-V+Vector+Migration;Building+Secure+Hardware+Systems;FPGA+%26+ASIC+Design;RISC-V+Processor+Architecture;Hardware+Security+Research" alt="Typing SVG" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/om-maheshwari-8a4996299/)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:omdaga6@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/om-mahesh)
![Profile Views](https://komarev.com/ghpvc/?username=om-mahesh&color=58a6ff&style=for-the-badge&label=Profile+Views)

</div>

---

## 🚀 About Me

I'm a **Hardware Engineer** and **VLSI Researcher** at **IIT Mandi**, working across processor architecture, FPGA/ASIC design, and hardware security. I like building systems that are **observable, efficient, and secure** from the RTL up — because **hardware is truth**.

- 🔭 **Flagship:** *Vector-Width Virtualization* — lossless cross-`VLEN` vector-task migration for RISC-V (see below)
- 🧠 Researching **RISC-V microarchitecture**, **neuromorphic / event-driven** compute, and **hardware security**
- 🔒 Building **hardware-based timing-attack detection**
- 💡 Passionate about **open-source hardware** and the **RISC-V ecosystem**
- 🎯 Core belief: **Hardware-first thinking, security-aware design**

---

## 🌟 Flagship Research — Vector-Width Virtualization (RISC-V)

> Making it possible to **correctly migrate a running vector task between RISC-V cores of different `VLEN`** — something stock RISC-V Linux silently corrupts today.

- 🧩 **Mechanism:** a non-destructive **effective vector-width cap** (`vlcap` CSR) — caps a wide core to a narrow *effective* width without touching register contents, so a task migrates losslessly to any core of `VLEN ≥ C`.
- 📐 **Theory:** a formal correctness condition + proof, including an `LMUL>1` **placement-confinement** soundness result.
- ⚙️ **Built across the whole stack:** reference implementations in **Spike, QEMU, gem5, and the Linux kernel**, with cross-engine **litmus tests** (validated for `LMUL ∈ {2,8}`).
- 📄 **Manuscript under submission** (IEEE TOC / ACM TACO) · **preparing an RFC for the RISC-V Vector SIG**.

`📦 Code & spec: public release in progress` <!-- replace with repo link when public -->

---

## 📚 Research & Publications

- **Vector-Width Virtualization for the RISC-V Vector Extension** — effective-width cap for lossless cross-`VLEN` task migration; proof + 4-engine reference implementation. *Under submission, 2026.*
- Hardware-based execution-time signatures for **real-time timing-attack detection** (microarchitectural security).

---

## 🛠️ Tech Stack

**Hardware Design & Architecture**

![Verilog](https://img.shields.io/badge/Verilog-00979D?style=for-the-badge&logo=verilog&logoColor=white)
![VHDL](https://img.shields.io/badge/VHDL-543978?style=for-the-badge)
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-00599C?style=for-the-badge)
![RISC-V](https://img.shields.io/badge/RISC--V-283272?style=for-the-badge&logo=riscv&logoColor=white)
![Xilinx](https://img.shields.io/badge/Xilinx_Vivado-E63946?style=for-the-badge&logo=xilinx&logoColor=white)

**Simulation & Modeling**

![gem5](https://img.shields.io/badge/gem5-2C3E50?style=for-the-badge)
![Spike](https://img.shields.io/badge/Spike_ISS-1C4E80?style=for-the-badge)
![QEMU](https://img.shields.io/badge/QEMU-FF6600?style=for-the-badge&logo=qemu&logoColor=white)
![ModelSim](https://img.shields.io/badge/ModelSim-1C4E80?style=for-the-badge)

**EDA Tools**

![Cadence](https://img.shields.io/badge/Cadence-0F5499?style=for-the-badge)
![Altium](https://img.shields.io/badge/Altium-A5915F?style=for-the-badge)
![Tanner EDA](https://img.shields.io/badge/Tanner_EDA-00599C?style=for-the-badge)

**Embedded & Programming**

![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![STM32](https://img.shields.io/badge/STM32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## 💼 Featured Projects

| Project | What it is | Stack |
|---|---|---|
| 🔒 **[Hardware ETS — Timing-Attack Detection](https://github.com/om-mahesh/Hardware-Based-Execution-Time-Signatures-ETS-for-Real-Time-Detection-of-Timing-Attacks)** | Real-time side-channel detection via execution-time profiling | `C` · Security |
| ⚡ **[Branch Prediction Unit (Optimized FSM)](https://github.com/om-mahesh/Branch-Prediction-Unit-with-Temporal-Properties-and-Optimized-FSM)** | Branch predictor with temporal properties | `Verilog` · Architecture |
| 🧠 **[Neuromorphic RISC-V](https://github.com/om-mahesh/neuromorphic-riscv)** | Event-driven / spike-based compute on RISC-V | `RISC-V` |
| 📡 **[FPGA Phase Unwrapping](https://github.com/om-mahesh/Efficient-FPGA-Based-Parallel-Phase-Unwrapping-Hardware-Architecture)** | Non-iterative DCT pipeline for holographic microscopy | `VHDL` · FPGA |
| 🧪 **[Power-Aware LBIST (MIPS32)](https://github.com/om-mahesh/Power-Aware-LBIST-for-a-MIPS32-Single-Cycle-Core)** | Power-aware built-in self-test for a processor core | `VHDL` · DFT |
| 🔬 **[Telescopic CMOS Op-Amp (180nm)](https://github.com/om-mahesh/Design-of-a-High-Speed-Low-Noise-Telescopic-CMOS-Operational-Amplifier-in-180-nm-Process)** | Full-custom analog design w/ DRC/LVS | Analog · Cadence |
| 📶 **[SmartRF](https://github.com/om-mahesh/SmartRF)** | RF signal classification with ML | DSP · ML |
| 🔧 **[Omduino X1](https://github.com/om-mahesh/Omduini-x1)** | Custom Arduino-class PCB (schematic → layout → assembly) | PCB · Embedded |

---

## 🔬 Research Interests

yaml
Computer Architecture:
  - RISC-V vector extension & cross-VLEN migration
  - Branch prediction, speculation, cache hierarchies
Hardware Security:
  - Side-channel analysis & timing-attack detection
  - Secure microarchitectures
FPGA & SoC Design:
  - Parallel pipelines, HLS, real-time signal processing
Neuromorphic Computing:
  - Event-driven processing, spiking networks in silicon
Verification:
  - Litmus testing, formal methods, BIST / DFT

---
📊 GitHub Analytics

<div align="center">

Om's GitHub Stats (https://github-readme-stats.vercel.app/api?username=om-mahesh&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=1F6FEB&text_color=C9D1D9&count_private=true)
Top Languages (https://github-readme-stats.vercel.app/api/top-langs/?username=om-mahesh&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=58A6FF&text_color=C9D1D9&langs_count=8)

GitHub Streak (https://github-readme-streak-stats.herokuapp.com/?user=om-mahesh&theme=tokyonight&hide_border=true&background=0D1117&ring=58A6FF&fire=58A6FF&currStreakLabel=C9D1D9)

Trophies (https://github-profile-trophy.vercel.app/?username=om-mahesh&theme=tokyonight&no-frame=true&no-bg=true&column=7&margin-w=4)

Activity Graph (https://github-readme-activity-graph.vercel.app/graph?username=om-mahesh&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=58A6FF&line=1F6FEB&point=C9D1D9)

</div>

---
🎯 Engineering Philosophy

▎ Hardware is truth. Software is proof.

🔹 Hardware-first — optimize at RTL, not as an afterthought  🔹 Every cycle & gate matters  🔹 Security built into silicon  🔹 Observable systems — what you can't measure, you can't trust  🔹 Verifiable correctness — simulation necessary, formal/litmus sufficient

🔹 Hardware-first — optimize at RTL, not as an afterthought  🔹 Every cycle & gate matters  🔹 Security built into silicon  🔹 Observable systems — what you can't measure, you can't trust  🔹 Verifiable correctness — simulation necessary, formal/litmus sufficient

---
<div align="center">

⚡ "Building tomorrow's processors, today" ⚡

LinkedIn (https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin) (https://www.linkedin.com/in/om-maheshwari-8a4996299/)
![Email](https://img.shields.io/badge/Email-omdaga6@gmail.com-D14836?style=for-the-badge&logo=gmail) (omdaga6@gmail.com)

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1F6FEB,100:0D1117&height=100&section=footer" />

</div>
