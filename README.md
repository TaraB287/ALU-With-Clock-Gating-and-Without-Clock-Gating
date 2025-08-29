# ALU-With-Clock-Gating-and-Without-Clock-Gating
A 4-bit ALU designed in Verilog with and without clock gating, verified in ModelSim and analyzed in Vivado.

This project implements a **4-bit Arithmetic Logic Unit (ALU)** in Verilog HDL.  
Two architectures are designed and analyzed:
1. **ALU with Clock Gating**  
2. **ALU without Clock Gating**

The project includes **functional simulation (ModelSim)** and **power/schematic analysis (Vivado)**.

##  Features
- Supports basic arithmetic and logical operations:
  - AND  
  - OR  
  - XOR  
  - ADD 
  - SUB  
  - Left Shift  
  - Right Shift
- Control signals select the operation (`cntrl[2:0]`).
- Implemented in two variants:
  - **With Clock Gating** – reduces dynamic power.  
  - **Without Clock Gating** – traditional design.

## Project Structure
```
├── src/                          # Verilog source files
│ ├── alu_4bit.v                  # Main ALU module
│ ├── alu_4bit_tb.v               # Testbench for ALU
├── simulation/  
│ └── modelsim_wave.jpg          # Simulation waveform results
├── synthesis/
│ ├── schematic_with_clk.jpg      # RTL schematic (with clock gating)
│ ├── schematic_without_clk.jpg   # RTL schematic (without clock gating)
│ ├── power_with_clk.jpg          # Power analysis (with clock gating)
│ └── power_without_clk.jpg       # Power analysis (without clock gating)
├── README.md
```

## Power Analysis (Vivado)
### With Clock Gating
- **Total On-Chip Power**: 2.264 W  
- Dynamic Power: 2.164 W (96%)  
- Static Power: 0.099 W  

### Without Clock Gating
- **Total On-Chip Power**: 2.244 W  
- Dynamic Power: 2.144 W (96%)  
- Static Power: 0.099 W  

## Results & Conclusion
- The **clock-gated ALU** shows **lower power consumption (2.244 W)** compared to the **non-clock-gated ALU (2.264 W)**.  
- This proves that **clock gating is effective in reducing dynamic power consumption**.  

##  Tools Used
- **ModelSim** – Functional simulation and waveforms.  
- **Vivado** – RTL analysis, synthesis, schematic, and power estimation.  

## Developed By 

- Tara Busaraddi
- Github : [TaraB287](https://github.com/TaraB287)
- LinkedIn : [tarabusarddi](https://www.linkedin.com/in/tarabusaraddi/)

  
