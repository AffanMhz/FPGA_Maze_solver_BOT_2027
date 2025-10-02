
# FPGA Maze Solver BOT 2027

An FPGA-based project repository for designing and simulating digital systems in **Verilog HDL** using **Intel Quartus** and **ModelSim**.  
This repository contains source code, constraints, simulations, and documentation for multiple tasks leading up to the implementation of a **maze-solving robot** on FPGA.

---

## 📂 Repository Structure
```

├── src/                # Verilog source files
├── constraints/        # Pin assignments, timing constraints
├── simulation/         # Testbenches, ModelSim outputs
├── fpga_projects/      # Quartus project files
├── scripts/            # Helper scripts (build/run)
├── docs/               # Documentation, diagrams
├── README.md           # Project overview
├── LICENSE             # Open-source license
├── .gitignore          # Ignore build/temp files
├── .gitattributes      # Line endings and text normalization

````

---

## 🎯 Problem Statements

### Task 1A — Frequency Scaling & PWM
- Input: 50 MHz clock  
- Output 1: 3.125 MHz clock  
- Output 2: 195 kHz PWM signal with 4-bit duty cycle control  

Deliverables:
- `frequency_scaling.v`  
- `pwm_generator.v`  
- Simulation waveforms verifying correct scaling & PWM  

---

### Task 1B — Ultrasonic Object Detection
- Sensor: HC-SR04  
- FSM-based Verilog controller  
- Outputs:
  - `obstacle` (high if object < 70 mm)  
  - `distance_out` (8-bit, mm)  

Deliverables:
- `t1b_ultrasonic.v`  
- Simulation testbench showing correct detection & distance calculation  

---

### Task 1C — RISC-V CPU (RV32I Subset)
- Implement a single-cycle RISC-V CPU in Verilog  
- Support all instructions listed in ISA spec  
- Use provided testbench (`tb.v`)  

Deliverables:
- `riscv_cpu.v`  
- Supporting modules (`alu.v`, `instr_mem.v`, `data_mem.v`, etc.)  
- Simulation outputs with correct instruction execution  

---

## ⚙️ Development Workflow
1. Clone the repo  
   ```bash
   git clone https://github.com/Affan1Mhz/FPGA_Maze_solver_BOT_2027.git
   cd FPGA_Maze_solver_BOT_2027
````

2. Create a feature branch

   ```bash
   git checkout -b task1a_pwm
   ```
3. Add your Verilog files under `src/` or Quartus project folder.
4. Push changes & make a Pull Request.

---

## 📖 Documentation

See the [`docs/`](./docs) folder for schematics, block diagrams, and notes.

---

## 👨‍💻 Team Members

* Affan (Team Lead)
* [Add your teammates here]
