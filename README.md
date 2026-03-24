

# Grover’s Algorithm using Qiskit

## Overview

This project implements Grover’s Search Algorithm using Qiskit. The program builds a quantum circuit with an oracle and diffusion operator, applies Grover iterations, and measures the result.


## Requirements

Make sure you have the following installed:

* Python (3.8 or above)
* Qiskit
* Matplotlib
* Jupyter Notebook (optional but recommended)

Install dependencies using:

```bash
pip install qiskit matplotlib notebook
```

---

## How to Run

### Step 1: Open the Notebook

Navigate to the project folder and run:

```bash
jupyter notebook
```

Open the file:

```
GQP_Grover_Qiskit_Project.ipynb
```

---

### Step 2: Run Cells

Run all cells in order from top to bottom.

This will:

* Define the oracle and diffusion functions
* Build the Grover circuit
* Execute the circuit
* Display results and circuit diagram

---

### Step 3: View Output

You will see:

* Circuit details (gate count, depth)
* Measurement results (probabilities of states)
* Visualization of the quantum circuit

---

## Notes

* Ensure that the number of qubits and target states are defined correctly.
* If the circuit diagram does not display, try:

  * Adding `%matplotlib inline` at the top of the notebook
  * Using `display(fig)` instead of `plt.show()`

---

## Troubleshooting

* Error: `barrier is not a gate instruction`

  * Solution: Avoid using `.to_gate()` on circuits that contain barriers. Use `.compose()` instead.

* Empty circuit output

  * Ensure oracle and diffusion circuits are correctly built and applied.

---

## File Structure

```
GQP_Grover_Qiskit_Project.ipynb
README.md
```


