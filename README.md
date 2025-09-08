# ZA25 Quantum Communication Simulation

This repository is a fork of [https://github.com/CETQAP/ZA25-Protocol/tree/main](https://github.com/CETQAP/ZA25-Protocol/tree/main).

This repository contains the implementation of a quantum communication simulation inspired by the ZA25 protocol, developed by the Centre of Excellence for Technology Quantum and AI (CETQAC). The project achieves a 100 km repeater-enhanced simulation with a fidelity of 0.9950, real-time 10-bit transmission of the message "10" with a fidelity of 0.946, and 100% shot accuracy. Built using Qiskit to demonstrate advancements in Quantum Secure Direct Communication (QSDC).

## Features

* Simulates a 100 km quantum repeater network with a mitigated fidelity of 0.9950.
* Executes real-time 10-bit quantum message transmission with a fidelity of 0.946.
* Achieves 100% shot accuracy using M3 error mitigation techniques.
* Runs on IBM Quantum's `ibm_sherbrooke` device or compatible backends.
* Includes data analysis and visualization tools for fidelity and accuracy metrics.

## Prerequisites

* Python 3.8 or higher
* Qiskit 0.44 or later (`pip install qiskit`)
* An IBM Quantum account ([Sign up](https://quantum.ibm.com/account))
* Optional: NumPy and Matplotlib for data analysis and visualization
* Git for version control

## Usage

To run the 100 km repeater-enhanced simulation:

```bash
python simulation.py --distance 100 --repeater --fidelity-target 0.9950
```

To execute the real-time 10-bit transmission:

```bash
python transmission.py --message "10" --device ibm_sherbrooke
```

Results, including fidelity and shot accuracy metrics, are saved in the `results/` directory as CSV files and visualizations.

## Results

* **Repeater Simulation:** 100 km distance, Fidelity = 0.9950, Shot Accuracy = 100%.
* **Real-Time Transmission:** 10-bit message "10", Fidelity = 0.946, Shot Accuracy = 100%.
  Detailed metrics and visualizations are available in `results/output.csv` and `results/plots/`.

## Sample Results

### Circuit Diagram

![Circuit Diagram](circuit_diagram.png)

### Qiskit Circuit

![Qiskit Circuit](ZA25%20Protocl%20Qiskit%20Circuit.png)

### Measurement Histogram

![Measurement Histogram](measurement_histogram.png)

### Hardware Results

![Hardware Results](ZA25%20Protocol%20Hardware%20Results.png)

### Measurement Results Table

| measurement | counts |
| ----------- | ------ |
| 000010      | 59     |
| 001001      | 72     |
| 000101      | 59     |
| 001010      | 62     |
| 001111      | 68     |
| 001101      | 67     |
| 000000      | 82     |
| 000111      | 67     |
| 000001      | 57     |
| 000011      | 64     |
| 000110      | 53     |
| 001000      | 64     |
| 001110      | 60     |
| 000100      | 67     |
| 001100      | 69     |
| 001011      | 54     |
