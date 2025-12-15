# SystemC Basic Examples

This repository contains **basic SystemC examples** intended for learning and practicing **SystemC modeling**, including module definition, simulation, events, and simple hardware-like components.

## Contents

### Documents

* **Ch1-SoC_CHN-Introduction&Défis.pdf**
  Introduction to SoC concepts, challenges, and SystemC motivation.

* **Ch2-SoC_CHN_ModelisationHw_Sw.pdf**
  Hardware/Software modeling concepts using SystemC.

* **TD1_SystemC.pdf**
  Tutorial/TD introducing SystemC basics with exercises.

### Directories (Examples)

* **systemC_installation/**
  Notes or scripts related to SystemC installation and setup.

* **HelloWorld/**
  Minimal SystemC example to verify installation and simulation flow.

* **adder/**
  Simple adder module illustrating:

  * `SC_MODULE`
  * Ports (`sc_in`, `sc_out`)
  * Combinational behavior

* **counter/**
  Counter example demonstrating:

  * Clocked processes
  * `SC_METHOD` / `SC_THREAD`
  * Reset and clock sensitivity

* **Bascule/**
  Flip-flop (bascule) example showing sequential logic modeling.

* **EX1_TD1/**
  Exercise 1 – introductory SystemC modeling tasks.

* **EX2_TD1/**
  Exercise 2 – intermediate concepts (processes, timing, signals).

* **EX3_TD1/**
  Exercise 3 – more advanced or combined SystemC behaviors.

* **exemple_event_slide_46/**
  Example illustrating **SystemC events (`sc_event`)** and synchronization between processes.

## Requirements

* SystemC library (2.3.x recommended)
* C++ compiler (GCC / Clang)
* Make or CMake (depending on example)

## How to Compile & Run (Typical)

```bash
export SYSTEMC_HOME=/path/to/systemc
export LD_LIBRARY_PATH=$SYSTEMC_HOME/lib-linux64

g++ -I$SYSTEMC_HOME/include \
    -L$SYSTEMC_HOME/lib-linux64 \
    main.cpp -lsystemc -o sim

./sim
```

> Check each folder for its own `main.cpp` or `Makefile` if provided.

## Learning Objectives

* Understand SystemC module structure
* Model combinational and sequential hardware
* Use clocks, resets, and events
* Run and analyze SystemC simulations


* Add **waveform tracing (VCD)** examples
* Clean and standardize all examples
