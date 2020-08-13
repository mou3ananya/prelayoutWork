# prelayoutWork
This repository contains a structural as well as functional description of a comparator and a clock divider with 3.3v analog voltage and 1.8v digital voltage. This repository will maintain simulation files and other relevant files on the pre-mentioned design blocks worked on in the Online VSD IP Design Research Internship program 2020.


*Note: Circuit requires further optimization to improve performance. Design yet to be modified.*

Table of contents
=================
<!--ts-->
   * [Block Diagram of the Comparator IP](#block-diagram-of-the-comparator-ip)
   * [Circuit Diagram of the Comparator IP](#circuit-diagram-of-the-comparator-ip)
   * [About Ngspice](#about-ngspice)
   * [Running the Simulation](#running-the-simulation)
   * [Pre-Layout Simulation](#pre-layout-simulation)
   * [Issues | Improvements | Future Work](#issues--improvements--future-work)
   * [A Glance at the Clock Divider IP](#a-glance-at-the-clock-divider-ip)
   * [Block Diagram of the Clock Divider IP](#block-diagram-of-the-clock-divider-ip)
   * [Circuit Diagram of the Clock Divider IP](#circuit-diagram-of-the-clock-divider-ip)
   * [Running the Simulation](#running-the-simulation)
   * [Pre-Layout Simulation](#pre-layout-simulation)
   * [Issues | Improvements | Future Work](#issues--improvements--future-work)
   * [Acknowledgments](#acknowledgments)
   * [Contact Information](#contact-information))
<!--te-->

## Block Diagram of the Comparator IP

<p align="center">
  <img width="800" height="500" src="/Images/comparator_block.PNG">
</p>

## CIRCUIT DIAGRAM of the Comparator IP

<p align="center">
  <img width="800" height="500" src="/Images/comparator_ckt.PNG">
</p>



<img align="left" width="60" height="50" src=/Images/ng_logo.PNG>

## About Ngspice 
Ngspice is an open source mixed-signal circuit simulator.

### Installing Ngspice

#### For Ubuntu

Open your terminal and type the following to install Ngspice
```
$  sudo apt-get install -y ngspice
```

## Running the Simulation


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

## Pre-Layout Simulation

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


## Issues | Improvements | Future Work

1. The biasing circuit is required some improvement in architecture since here I'm using 2Meg resister which is more area as well as power comsuming compare to MOS transister.
2. The current comparator can detect the difference between Vp(Non-inverting) and Vn(Inverting) i/p terminal voltage upto 20mv which needs an improvement upto 3.2mv to meet 
   the specs of 10bit ADC IP[here](/Documentation/Specifications.pdf).
   
   
   
## Block Diagram of the Clock Divider IP

<p align="center">
  <img width="800" height="500" src="/Images/clkdivider_block.PNG">
</p>

## CIRCUIT DIAGRAM of the Comparator IP

<p align="center">
  <img width="800" height="500" src="/Images/clkdivider_circuit.png">
</p>

## Running the Simulation


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
## Pre-Layout Simulation

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


## Issues | Improvements | Future Work

Output pulse is of 33% duty cycle since I've used one 3bit asynchronous up-counter followed by a MOD-3 asynchronous up counter. I'll modify the circuit to get 50% duty cycle
which is important to meet the 10bit ADC IP spec[here](/Documentation/Specifications.pdf).


## Contributors 

- **Ananya Ghorai** 
- **Kunal Ghosh** 

## Acknowledgments
- Kunal Ghosh, Director, VSD Corp. Pvt. Ltd.
- Philipp Gühring, Software Architect, LibreSilicon Assocation


## Contact Information

- Ananya Ghorai, Pursuing M.Tech in VLSI Design, IIT(ISM) Dhanbad, ananyaghorai.2012@gmail.com
- Kunal Ghosh, Director, VSD Corp. Pvt. Ltd. kunalghosh@gmail.com
- Philipp Gühring, Software Architect, LibreSilicon Assocation pg@futureware.at
