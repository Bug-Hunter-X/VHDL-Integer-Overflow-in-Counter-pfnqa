# VHDL Integer Overflow Bug

This repository demonstrates a common bug in VHDL code: integer overflow in a counter. The provided VHDL code implements a simple counter that increments on each rising edge of a clock signal. However, it does not handle the case when the counter reaches its maximum value (15 in this case), resulting in an unexpected wrap-around behavior.

The `bug.vhdl` file contains the erroneous code. The `bugSolution.vhdl` file offers a corrected version that prevents the overflow by adding a check to stop the counter at the maximum value.

## How to reproduce

1. Simulate the provided VHDL code using a suitable VHDL simulator (e.g., ModelSim, GHDL).
2. Observe the counter's behavior when it reaches 15.  It should wrap around to 0 instead of stopping.