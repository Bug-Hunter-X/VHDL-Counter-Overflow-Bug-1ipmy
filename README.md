# VHDL Counter Overflow Bug

This repository demonstrates an uncommon bug in VHDL related to integer overflow in a simple counter.

## Bug Description
The `buggy_counter.vhdl` file contains a counter that increments on each rising clock edge.  The issue arises when the counter reaches its maximum value (15).  A naive reset back to 0 might lead to unexpected behaviour or simulation errors if not handled with precise timing and signal updates.

## Solution
The `fixed_counter.vhdl` demonstrates a solution addressing the integer overflow handling within the process. The corrected code ensures the counter resets reliably to zero after reaching the maximum value, avoiding any inconsistencies.