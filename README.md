

# 🖥️ MIPS Processor Design using VHDL – Full Project

**Course:** CESS3005 – Computer Architecture
**University:** Ain Shams University – Faculty of Engineering
**Department:** Computer Engineering and Software Systems


## 📌 Project Overview

This project demonstrates the design and simulation of a simplified **MIPS processor** using **VHDL**, structured in **two phases**:

* ✅ **Phase I**: Building the Register File, ALU, and the Datapath for R-type instructions.
* ✅ **Phase II**: Extending the processor to support I-type (`lw`, `sw`, `beq`) and J-type (`j`) instructions, integrating memory modules and the control unit.

---



## 📁 Directory Structure

```
/MIPS_Processor_VHDL_Project
│
│   ├── register_file.vhd
│   ├── alu.vhd
│   ├── control_unit.vhd
│   ├── datapath.vhd
│   ├── instruction_memory.vhd
│   ├── data_memory.vhd
│   ├── mips.vhd
│   └── top_level.vhd
│

│   └── mips_testbench.vhd
│

├── 1_CESS3005_CSE112_Major_Task_students_Ver2.pdf
└── README.md
```

---

## 📐 Phase I Summary

### ✅ Implemented Components:

* **Register File**:

  * Simultaneous read from two registers, write to one
  * `RegisterFile` entity with full 32-register support
* **ALU**:

  * Supports `AND`, `OR`, `ADD`, `SUB`, `NOR`
  * Zero flag output
* **Datapath**:

  * Executes R-type instructions (`add`, `sub`, `and`, `or`, `nor`, `slt`)

### ✅ Deliverables:

* VHDL code for all modules
* Testbench verifying all supported R-type operations
* Simulation waveforms

---

## 🧩 Phase II Summary

### ✅ Extended Functionality:

* **Control Unit**: Generates control signals for full instruction set
* **Instruction & Data Memory**: Simulated with simple program
* **I-type Support**: `lw`, `sw`, `beq`
* **J-type Support**: `j`
* **Top-level `mips` module** integrates datapath + control + memory

### ✅ Test Case Program:

A sample program is loaded in memory to:

1. Load values into registers from memory
2. Perform arithmetic and logic operations
3. Store results back to memory
4. Branch and jump based on conditions

---

## 📄 Report Contents

Available in `docs/Final_Project_Report.pdf`, includes:

* 📘 Project Description & Requirements
* 🔧 Implementation Details (with schematics)
* 🧠 Design Decisions & Assumptions
* 📊 Simulation Screenshots
* 🧪 Test Program & Sample Outputs
* 👥 Contribution Breakdown (who did what)

---

## 🧪 Simulation Tools

* VHDL Simulated using **ModelSim** or **QuestaSim**
* Waveforms and behavioral outputs observed and verified


