#  AXI Protocol Utilities – Burst & WSTRB Calculation

This repository provides two Python scripts designed to automate critical AXI protocol-related calculations often used in FPGA/ASIC verification environments. Both tools are tailored for **aligned address scenarios** and help improve efficiency, accuracy, and reusability in testbench development.

---

##  Tool 1: AXI Burst Calculator

###  Description
This script calculates the **AXI burst boundaries and next address** based on user input. It is especially useful during testbench development to validate address alignment and burst behavior.

###  Inputs:
- `start_address`: Starting address of the burst
- `size`: Size of the data to transfer
- `burst_length`: Number of data beats in the burst

###  Outputs:
The script generates a `.txt` file containing:
- Start Address  
- Lower Boundary  
- Upper Boundary  
- Next Address  

---

##  Tool 2: AXI WSTRB (Strobe) Calculator

###  Description
This script computes the **WSTRB (write strobe)** signal for AXI/AXI-Lite write transactions. It's useful for checking correct byte lane activation during aligned transfers.

###  Inputs:
- `no_byte_lane`: Number of byte lanes in the bus
- `start_address`: Aligned start address
- `size`: Total size of the transfer
- `burst_length`: Number of beats

###  Outputs:
The script generates a `.txt` file containing:
- Start Address  
- Number of Byte Lanes  
- Size  
- Generated WSTRB pattern  

---

##  Note:
Both tools assume **aligned address inputs**. They are ideal for testbench development, protocol checking, or educational purposes in the VLSI design and verification space.

---

##  How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/axi-burst-wstrb-tools.git
   cd axi-burst

