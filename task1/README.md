Task-1: Environment Setup & RISC-V Reference Validation

ENVIRONMENT  
GitHub Codespace (Linux)

RISC-V REFERENCE PROGRAM  
Repository: vsd-riscv2  
Program Location: samples/  

The reference RISC-V program was successfully compiled and executed using the Spike simulator.  
The output confirmed correct execution of the program logic.

VSDFPGA LABS  
Repository: vsdfpga_labs  
Lab Executed: basic RISC-V firmware build  

The firmware build completed successfully and the memory initialization file was generated.  
FPGA bitstream generation and hardware flashing were intentionally skipped as per task instructions.

UNDERSTANDING CHECK  

1. Where is the RISC-V program located in the vsd-riscv2 repository?  
The reference RISC-V program is available inside the `samples` directory of the vsd-riscv2 repository.

2. How is the program compiled and loaded into memory?  
The program is compiled using the RISC-V cross-compilation toolchain and executed through the Spike simulator, which loads the compiled binary into simulated memory.

3. How does the RISC-V core access memory and memory-mapped IO?  
The RISC-V core accesses memory and peripherals using standard load and store instructions over the system interconnect.

4. Where would a new FPGA IP block logically integrate in this system?  
A new FPGA IP block would be integrated as a memory-mapped peripheral on the system bus, allowing the RISC-V core to communicate with it through defined address ranges.

NOTE  
All tasks were executed entirely within GitHub Codespace. FPGA synthesis, bitstream generation, and hardware flashing were not performed for Task-1.

