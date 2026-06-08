# Quantum Adders using Qiskit

This repository contains Qiskit implementations and analysis of four exact quantum adder architectures:

- Vedral-Barenco-Ekert (VBE) Adder
- Cuccaro Ripple-Carry Adder
- Thapliyal Adder
- Seo Adder

These implementations are based on the architectures presented in:

> **Fig. 1. Circuit schemes of 4-qubit exact quantum adders:**  
> (a) Vedral, (b) Cuccaro, (c) Thapliyal, and (d) Seo.


---

## Overview

Quantum adders are essential components of quantum arithmetic and form the basis of many quantum algorithms. This project implements and compares multiple exact quantum adder architectures using Qiskit and evaluates their performance under realistic quantum noise models.

---

## Implemented Adders

### 1. Vedral-Barenco-Ekert (VBE) Adder
- Ripple-carry based design
- Uses carry and sum computation stages
- One of the earliest quantum adder architectures

### 2. Cuccaro Adder
- Efficient ripple-carry adder
- Reduced ancilla qubit requirements
- Widely used in quantum arithmetic circuits

### 3. Thapliyal Adder
- Optimized reversible adder architecture
- LCA 
- Improved gate efficiency

### 4. Seo Adder
- Exact quantum adder design
- Optimized for quantum circuit implementation
- Efficient RCA

---

## Features

- 4-bit exact quantum addition
- Reversible circuit implementation
- Qiskit-based simulation
- Noise-aware circuit evaluation
- Automated testing for all input combinations
- Comparative analysis of adder architectures

---

## Noise Models

The following quantum noise models are supported:

- Depolarizing Noise
- Bit-Flip Noise
- Phase-Flip Noise

Noise simulations are performed using **Qiskit Aer**.

---

## Error Metrics

Circuit reliability is evaluated using:

### Error Rate (ER)

Measures the probability of obtaining an incorrect output.

### Normalized Mean Error Distance (NMED)

Measures the average output deviation normalized by the maximum possible error.

### Mean Relative Error Distance (MRED)

Measures the average relative error with respect to the correct output.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/devStormAkash/Quantum-Adder.git
```

Install dependencies:

```bash
pip install qiskit qiskit-aer numpy matplotlib
```

---

## Project Structure

```text
quantum-adders/
│
├── vedral/
│   ├── vedral_adder.py
│
├── cuccaro/
│   ├── cuccaro_adder.py
│
├── thapliyal/
│   ├── thapliyal_adder.py
│
├── seo/
│   ├── seo_adder.py
│
│
└── README.md
```

---

## Applications

- Quantum Arithmetic
- Reversible Computing
- Quantum Algorithm Design
- NISQ Circuit Analysis
- Fault-Tolerant Quantum Computing Research

---

## Future Work

- Extension to n-bit adders
- Hardware execution on real quantum processors
- Circuit optimization and transpilation studies
- Fault-tolerant implementations
- Quantum cost and depth analysis

---

## References

1. Vedral, V., Barenco, A., and Ekert, A.
   *Quantum Networks for Elementary Arithmetic Operations.*

2. Cuccaro, S. A., Draper, T. G., Kutin, S. A., and Moulton, D. P.
   *A New Quantum Ripple-Carry Addition Circuit.*

3. Thapliyal, H., and Ranganathan, N.
   *Design of Efficient Reversible Lookahead-Carry Adder and BCD Adder Circuits.*

4. Seo et al.
   *Exact Quantum Ripple Carry Adder Architecture.*

---

## Author

**Akash Giri**  
National Institute of Technology Durgapur
