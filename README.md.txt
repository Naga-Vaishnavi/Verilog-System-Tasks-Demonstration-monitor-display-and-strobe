🔍 Description

This project illustrates how $monitor, $display, and $strobe behave differently during simulation when variable values change. A simple Verilog module is used to show when and how each task prints output.

🎯 Importance

Essential for debugging and verification in Verilog simulations

Helps understand simulation time control and event scheduling

Commonly asked topic in VLSI interviews and labs

🛠️ Needs

Basic knowledge of Verilog HDL

Any Verilog simulator (ModelSim, Questa, Vivado, EDA Playground)

🧠 Key Concepts

$monitor → Continuously prints whenever a variable changes

$display → Prints immediately at the statement execution time

$strobe → Prints at the end of the current simulation time step

🧪 Example
a = 2; b = 3;
#5 $display(...);

a = 6; b = 7;
$strobe(...);


This shows how $display prints instantly, while $strobe waits until the time slot ends.

🗂️ Project Structure
├── system_tasks.v   // Verilog module demonstrating system tasks
└── README.md        // Project documentation

🚀 Future Scope

Add waveform dumping ($dumpfile, $dumpvars)
Extend examples with clocked processes
Compare with SystemVerilog equivalents

## 🛠 How to Run Simulation Using EDA tool

Add both design files and the testbench to your Verilog simulator
Compile and Run

✅ Conclusion

This project provides a clear and beginner-friendly explanation of Verilog system tasks, making it easier to debug simulations and understand timing behavior in digital design.