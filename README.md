<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1F6FEB,100:58A6FF&height=210&section=header&text=Om%20Maheshwari&fontColor=ffffff&fontSize=52&animation=fadeIn&fontAlignY=34&desc=Hardware%20Engineer%20%E2%80%A2%20VLSI%20Researcher%20%E2%80%A2%20RISC-V&descAlignY=56&descSize=18" />

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=680&lines=Lossless+RISC-V+Vector+Migration;From+RTL+to+ISA+to+Kernel;FPGA+%26+ASIC+%2F+Full-Custom+VLSI;Hardware+Security+%26+Side-Channels;Synthesizing+the+future%2C+one+gate+at+a+time" alt="Typing SVG" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/om-maheshwari-8a4996299/)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:omdaga6@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/om-mahesh)
![Profile Views](https://komarev.com/ghpvc/?username=om-mahesh&color=58a6ff&style=for-the-badge&label=Profile+Views)

</div>

```systemverilog
// who_am_i.sv  —  synthesizable, verified, side-channel-aware
module om_maheshwari #(
    parameter string ROLE = "Hardware Engineer / VLSI Researcher",
    parameter string ORG  = "IIT Mandi"
) (
    input  logic        clk,            // always running, always learning
    input  logic        rst_n,
    output logic [63:0]  silicon
);
    localparam CREED = "Hardware is truth. Software is proof.";

    always_ff @(posedge clk or negedge rst_n)
        if (!rst_n) silicon <= '0;
        else        silicon <= design(.secure(1), .observable(1), .efficient(1));

    // synthesis: RTL -> ISA -> kernel.  no level left as an afterthought.
endmodule
```

<div align="center">

```text
        ┌────┐    ┌────┐    ┌────┐    ┌────┐    ┌────┐
 clk  ──┘    └────┘    └────┘    └────┘    └────┘    └──
        ┌─────────┐         ┌──────────────────┐
 idea ──┘  RTL    └──ISA────┘     SILICON       └────────
              ▲ design   ▲ verify   ▲ ship
```

</div>

---

## 🚀 About Me

**Hardware Engineer & VLSI Researcher @ IIT Mandi.** I build computing systems that are **observable, efficient, and secure** — all the way down. My work spans **RISC-V microarchitecture, full-custom & FPGA design, and hardware security**, and I'm happiest with a waveform viewer open and a synthesis report compiling.

- 🔭 **Flagship:** *Vector-Width Virtualization* — lossless cross-`VLEN` vector-task migration for RISC-V *(below)*
- 🧠 RISC-V cores · neuromorphic / event-driven compute · side-channel defense
- 🔒 Hardware-based timing-attack detection in silicon
- 💡 Open-source hardware & the RISC-V ecosystem
- 🎯 **Hardware-first thinking, security-aware design**

---

## 🌟 Flagship Research — Vector-Width Virtualization (RISC-V)

> Make a running vector task **migrate correctly between RISC-V cores of different `VLEN`** — something stock RISC-V Linux silently corrupts today (a 512→128 move leaves only **2 of 32** registers intact, no trap).

```text
   ┌──────────────── 512-bit VPU ────────────────┐        ┌─ 128-bit VPU ─┐
   │ v0 [■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■]  │  vlcap │ v0 [■■■■■■■■] │
   │ ...                          (full width)    │  ═══▶  │ ...  (cap C)  │
   └──────────────────────────────────────────────┘  cap  └───────────────┘
        task running wide  ──── migrates losslessly ────▶  runs on narrow core
```

- 🧩 **Mechanism:** a **non-destructive** effective-width cap (`vlcap` CSR) — a wide core presents a narrow *effective* width without touching register contents.
- 📐 **Theory:** formal correctness condition + proof, incl. the `LMUL>1` **placement-confinement** soundness result.
- ⚙️ **Full-stack build:** reference implementations in **Spike · QEMU · gem5 · Linux kernel**, with cross-engine **litmus tests** (validated for `LMUL ∈ {2,8}`).
- 📄 **Manuscript under submission** (IEEE TOC / ACM TACO) · **preparing an RFC for the RISC-V Vector SIG**.

`📦 code & spec: public release in progress`  <!-- replace with repo link when public -->

---

## 📚 Research & Publications

- **Vector-Width Virtualization for the RISC-V Vector Extension** — effective-width cap for lossless cross-`VLEN` task migration; proof + 4-engine reference implementation. *Under submission, 2026.*
- **Hardware Execution-Time Signatures (ETS)** — real-time microarchitectural timing-attack detection.

---

## 🧰 Tech Stack

<div align="center">

**RTL & Architecture**

![Verilog](https://img.shields.io/badge/Verilog-00979D?style=for-the-badge&logo=verilog&logoColor=white)
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-00599C?style=for-the-badge)
![VHDL](https://img.shields.io/badge/VHDL-543978?style=for-the-badge)
![RISC--V](https://img.shields.io/badge/RISC--V-283272?style=for-the-badge&logo=riscv&logoColor=white)
![Chisel](https://img.shields.io/badge/Chisel-DD2A1B?style=for-the-badge)

**VLSI / EDA — Digital & Analog**

![Cadence](https://img.shields.io/badge/Cadence_Virtuoso-0F5499?style=for-the-badge)
![Synopsys](https://img.shields.io/badge/Synopsys-3B4CC0?style=for-the-badge)
![Vivado](https://img.shields.io/badge/Xilinx_Vivado-E63946?style=for-the-badge&logo=xilinx&logoColor=white)
![ModelSim](https://img.shields.io/badge/ModelSim-1C4E80?style=for-the-badge)
![Tanner](https://img.shields.io/badge/Tanner_EDA-00599C?style=for-the-badge)
![OpenLane](https://img.shields.io/badge/OpenLane-2E8B57?style=for-the-badge)
![KLayout](https://img.shields.io/badge/KLayout-6A5ACD?style=for-the-badge)

**Architecture Simulation**

![gem5](https://img.shields.io/badge/gem5-2C3E50?style=for-the-badge)
![Spike](https://img.shields.io/badge/Spike_ISS-1C4E80?style=for-the-badge)
![QEMU](https://img.shields.io/badge/QEMU-FF6600?style=for-the-badge&logo=qemu&logoColor=white)

**Embedded & Boards**

![STM32](https://img.shields.io/badge/STM32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-000000?style=for-the-badge&logo=espressif&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Altium](https://img.shields.io/badge/Altium_PCB-A5915F?style=for-the-badge&logo=altiumdesigner&logoColor=white)

**Software**

![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![TCL](https://img.shields.io/badge/TCL-FF5C00?style=for-the-badge)

</div>

---

## 💼 Featured Projects

| Project | What it is | Stack |
|---|---|---|
| 🌐 **Vector-Width Virtualization (RISC-V)** ⭐ | Lossless cross-`VLEN` vector migration: `vlcap` CSR + proof + Spike/QEMU/gem5/Linux | RISC-V · ISA · Kernel |
| 🔒 **[Hardware ETS — Timing-Attack Detection](https://github.com/om-mahesh/Hardware-Based-Execution-Time-Signatures-ETS-for-Real-Time-Detection-of-Timing-Attacks)** | Real-time side-channel detection via execution-time profiling | `C` · Security |
| ⚡ **[Branch Prediction Unit (Optimized FSM)](https://github.com/om-mahesh/Branch-Prediction-Unit-with-Temporal-Properties-and-Optimized-FSM)** | Branch predictor with temporal properties | `Verilog` · uArch |
| 🧠 **[Neuromorphic RISC-V](https://github.com/om-mahesh/neuromorphic-riscv)** | Event-driven / spike-based compute on RISC-V | RISC-V |
| 📡 **[FPGA Phase Unwrapping](https://github.com/om-mahesh/Efficient-FPGA-Based-Parallel-Phase-Unwrapping-Hardware-Architecture)** | Non-iterative DCT pipeline for holographic microscopy | `VHDL` · FPGA |
| 🧪 **[Power-Aware LBIST (MIPS32)](https://github.com/om-mahesh/Power-Aware-LBIST-for-a-MIPS32-Single-Cycle-Core)** | Power-aware built-in self-test for a CPU core | `VHDL` · DFT |
| 🔬 **[Telescopic CMOS Op-Amp (180nm)](https://github.com/om-mahesh/Design-of-a-High-Speed-Low-Noise-Telescopic-CMOS-Operational-Amplifier-in-180-nm-Process)** | Full-custom analog w/ DRC/LVS + post-layout | Analog · Cadence |
| 📶 **[SmartRF](https://github.com/om-mahesh/SmartRF)** | RF signal classification with ML | DSP · ML |
| 🔧 **[Omduino X1](https://github.com/om-mahesh/Omduini-x1)** | Custom Arduino-class PCB (schematic → layout → assembly) | PCB · Embedded |

---

## 🔬 Research Interests

```yaml
Computer Architecture:
  - RISC-V vector extension & cross-VLEN task migration
  - Branch prediction, speculation, cache hierarchies
VLSI / Physical Design:
  - Full-custom analog (op-amps), digital RTL-to-GDSII
  - DFT / BIST, low-power & power-aware testing
Hardware Security:
  - Side-channel analysis & timing-attack detection
  - Secure, observable microarchitectures
FPGA & SoC:
  - Parallel pipelines, HLS, real-time DSP
Neuromorphic:
  - Event-driven processing, spiking networks in silicon
```

---

## 📊 GitHub Analytics

<div align="center">

![Stats](https://github-readme-stats.vercel.app/api?username=om-mahesh&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=1F6FEB&text_color=C9D1D9&count_private=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=om-mahesh&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=58A6FF&text_color=C9D1D9&langs_count=8)

![Streak](https://github-readme-streak-stats.herokuapp.com/?user=om-mahesh&theme=tokyonight&hide_border=true&background=0D1117&ring=58A6FF&fire=58A6FF&currStreakLabel=C9D1D9)

![Trophies](https://github-profile-trophy.vercel.app/?username=om-mahesh&theme=tokyonight&no-frame=true&no-bg=true&column=7&margin-w=4&margin-h=4)

![Activity](https://github-readme-activity-graph.vercel.app/graph?username=om-mahesh&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=58A6FF&line=1F6FEB&point=C9D1D9&area=true)

<!-- Snake animation (enable the snake.yml GitHub Action to generate this) -->
<img src="https://raw.githubusercontent.com/om-mahesh/om-mahesh/output/github-contribution-grid-snake-dark.svg" alt="contribution snake" />

</div>

---

## 🧪 Engineering Philosophy

```systemverilog
// every design ships with its assertions
property hardware_first;  @(posedge clk) optimize |-> at_rtl_level;  endproperty
property secure_by_design;@(posedge clk) compute  |-> defended_in_silicon;  endproperty
property observable;      @(posedge clk) trust     |-> measurable;  endproperty

assert property (hardware_first);    // optimize at RTL, not as an afterthought
assert property (secure_by_design);  // defense belongs in the gates
assert property (observable);        // what you can't measure, you can't trust
// simulation is necessary; formal + litmus is sufficient.
```

---

<div align="center">

### ⚡ "Building tomorrow's processors, today" ⚡

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/om-maheshwari-8a4996299/)
[![Email](https://img.shields.io/badge/Email-omdaga6@gmail.com-D14836?style=for-the-badge&logo=gmail)](mailto:omdaga6@gmail.com)

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:58A6FF,50:1F6FEB,100:0D1117&height=110&section=footer" />

</div>
