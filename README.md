# VLSIDesign_8bitAdder
VLSI layout and spice netlist for an 8-bit ripple carry adder

## Running Netgen
To extract the magic layout:
```
% set vdd Vdd
% set gnd GND
% set Gnd GND
% extract
% ext2spice
% ext2sim
```

## Running Layout vs Schematic (LVS)
```
lvs FA.spc FA.spice FA.tcl FA.out
lvs ADDER.fspc ADDER.spice ADDER.tcl ADDER.out
```
## Running IRSIM
```
irsim scmos30.prm FA.sim -FA.cmd
irsim scmos30.prm ADDER.sim -ADDER.cmd
```
