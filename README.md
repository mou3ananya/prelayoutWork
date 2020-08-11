# prelayoutWork
This repository contains a structural as well as functional description of a comparator and a clock divider with 3.3v analog voltage and 1.8v digital voltage. It also contains the functional outcome of an integrated block consisting of a sample &amp; hold and the comparator along with another integrated block consisting of the clock divider and the sample &amp; hold. This repository will maintain simulation files and other relevant files on the pre-mentioned design blocks worked on in the Online VSD IP Design Research Internship 2020
## COMPARATOR BLOCK
### BLOCK DIAGRAM
<p align="center">
  <img width="800" height="500" src="/Images/comparator_block.PNG">
</p>

### CIRCUIT DIAGRAM
<p align="center">
  <img width="800" height="500" src="/Images/comparator_circuit.PNG">
</p>


### About Ngspice 
Ngspice is an open source mixed-signal circuit simulator.

#### Installing Ngspice

##### For Ubuntu

Open your terminal and type the following to install Ngspice
```
$  sudo apt-get install -y ngspice
```

### Running the Simulation


To enter the Ngspice Shell, open the terminal & type:
```
$ ngspice
```
To simulate a netlist, type:
```
ngspice 1 ->  source <filename>.cir
```

You can exit from the Ngspice Shell by typing:
```
ngspice 1 ->  exit
```
 <p align="center"> or </p>
 
```
ngspice 1 ->  quit
```
#### Pre-Layout Simulation

To clone the Repository and download the Netlist files for Simulation, enter the following commands in your terminal.

```
$  sudo apt install -y git
$  git clone https://github.com/mou3ananya/prelayoutWork
$  cd prelayoutWork/comparator
```
Run the netlist file using the following command.
```
$  ngspice comparator.cir
```


<p align="center">
 <img width="800" height="500" src="/Images/Comparator.PNG">
</p>

## CLOCK DIVIDER BLOCK
### BLOCK DIAGRAM
<p align="center">
  <img width="800" height="500" src="/Images/clkdivider_block.PNG">
</p>

### CIRCUIT DIAGRAM
<p align="center">
  <img width="800" height="500" src="/Images/clkdivider_circuit.png">
</p>


### About Ngspice 
Ngspice is an open source mixed-signal circuit simulator.

#### Installing Ngspice

##### For Ubuntu

Open your terminal and type the following to install Ngspice
```
$  sudo apt-get install -y ngspice
```

### Running the Simulation


To enter the Ngspice Shell, open the terminal & type:
```
$ ngspice
```
To simulate a netlist, type:
```
ngspice 1 ->  source <filename>.cir
```

You can exit from the Ngspice Shell by typing:
```
ngspice 1 ->  exit
```
 <p align="center"> or </p>
 
```
ngspice 1 ->  quit
```
#### Pre-Layout Simulation

To clone the Repository and download the Netlist files for Simulation, enter the following commands in your terminal.

```
$  sudo apt install -y git
$  git clone https://github.com/mou3ananya/prelayoutWork
$  cd prelayoutWork/clkdivider
```
Run the netlist file using the following command.
```
$  ngspice clk_divider.cir
```


<p align="center">
 <img width="800" height="500" src="/Images/clk_divider.PNG">
</p>

## PRE-LAYOUT SIMULATION FOR COMBINED SAMPLE & HOLD AND COMPARATOR CIRCUIT

To clone the Repository and download the Netlist files for Simulation, enter the following commands in your terminal.

```
$  sudo apt install -y git
$  git clone https://github.com/mou3ananya/prelayoutWork
$  cd prelayoutWork/Combined_sample_comparator
```
Run the netlist file using the following command.
```
$  ngspice sample_comp.cir
```


<p align="center">
 <img width="800" height="500" src="/Images/combined_sample_comparator.PNG">
</p>

## PRE-LAYOUT SIMULATION FOR COMBINED CLOCK DIVIDER, SAMPLE & HOLD AND COMPARATOR CIRCUIT

To clone the Repository and download the Netlist files for Simulation, enter the following commands in your terminal.

```
$  sudo apt install -y git
$  git clone https://github.com/mou3ananya/prelayoutWork
$  cd prelayoutWork/sample_comparator_clkdivider
```
Run the netlist file using the following command.
```
$  ngspice sample_comp_clk.cir
```


<p align="center">
 <img width="800" height="500" src="/Images/sample_comp_clk.PNG">
</p>

## Acknowledgments
- Kunal Ghosh, Director, VSD Corp. Pvt. Ltd.
- Philipp Gühring, Software Architect, LibreSilicon Assocation


## Contact Information

- Ananya Ghorai, Pursuing M.Tech in VLSI Design, IIT(ISM) Dhanbad, ananyaghorai.2012@gmail.com
- Kunal Ghosh, Director, VSD Corp. Pvt. Ltd. kunalghosh@gmail.com
- Philipp Gühring, Software Architect, LibreSilicon Assocation pg@futureware.at
