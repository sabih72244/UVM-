# APB Bus Master Verification using UVM

## 📌 Overview

This project implements a simple **UVM-based verification environment for an APB Bus Master** using **SystemVerilog**.

The main purpose of this lab is to understand the basic UVM verification flow and how transactions are transferred from a sequence to the DUT through a driver and observed using a monitor.

The project is intentionally designed with **simple and beginner-friendly logic**.

---

## 🎯 Objectives

- Create a simple UVM agent for an APB bus master.
- Generate APB transactions using a UVM sequence.
- Transfer transactions from Sequence → Sequencer → Driver.
- Drive APB signals to the DUT.
- Monitor and collect APB transactions.
- Understand the basic structure of a UVM testbench.
- Simulate the design using EDA Playground.

---

## 🛠️ Technologies Used

- **SystemVerilog**
- **UVM (Universal Verification Methodology)**
- **APB (Advanced Peripheral Bus)**
- **EDA Playground**
- **EPWave** for waveform visualization

---

## 🔄 UVM Verification Flow

The basic transaction flow used in this project is:

```text
       Sequence
           ↓
       Sequencer
           ↓
         Driver
           ↓
         APB DUT
           ↓
        Monitor
