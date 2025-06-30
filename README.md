
#  Phython Script - Burst Calculation & Strobe Calculation

This repository provides two Python scripts designed to automate critical AXI & AHB protocol-related calculations often used in FPGA/ASIC verification environments. Both script improve efficiency, accuracy, and reusability in testbench development.

---

##  Script 1: Burst Calculator

###  Description
This script calculates the **Burst boundaries and next address** based on user input. It is especially useful during testbench development to validate address alignment and burst behavior.

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

##  Script 2: Strobe Calculator

###  Description
This script computes the **Strobe** signal for AXI & AHB write transactions. It's useful for checking correct byte lane activation during transfers.

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

#  How to Use
-> Clone this repository:
   - Strobe_cal.exe
   - burst_calc.exe
   - git clone https://github.com/janak-dj/AMBA_strobe_burst_script.git
   - cd AMBA_Strobe_burst_script.git
   - [Python_Scriopt_Auto_Burst_Strobe_Calc.pdf](https://github.com/user-attachments/files/20973756/Python_Scriopt_Auto_Burst_Strobe_Calc.pdf)

