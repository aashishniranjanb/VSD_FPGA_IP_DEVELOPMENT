# Task-1: Understanding Check

## 1. Where is the RISC-V program located in the `vsd-riscv2` repository?
The RISC-V program is located in the software source directory of the `vsd-riscv2` repository, which contains the C or assembly files used as the reference application executed by the RISC-V core.

## 2. How is the program compiled and loaded into memory?
The program is compiled using the RISC-V cross-compilation toolchain provided in the GitHub Codespace. The generated binary is then loaded into the instruction memory through the build and run flow defined in the repository Makefile or scripts, simulating firmware loading.

## 3. How does the RISC-V core access memory and memory-mapped IO?
The RISC-V core accesses memory and peripherals using standard load and store instructions. Memory-mapped IO devices are assigned specific address ranges, allowing the core to communicate with peripherals using normal memory read and write operations.

## 4. Where would a new FPGA IP block logically integrate in this system?
A new FPGA IP block would integrate as a memory-mapped peripheral connected to the RISC-V core’s bus or interconnect. It would be assigned a unique address space so the processor can control and communicate with it using load/store instructions.
