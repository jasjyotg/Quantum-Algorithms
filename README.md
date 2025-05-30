
#  Quantum Algorithms with Qiskit

This project implements two of the most foundational quantum algorithms using IBM's Qiskit framework:

-  **Shor’s Algorithm** for integer factorization  
-  **Grover’s Algorithm** for unstructured database search

Each notebook walks through the logic, circuit design, and execution of the algorithm on a quantum simulator, with commentary and visualization.

---

##  Shor’s Algorithm – Factorization

Shor’s algorithm : factor large integers exponentially faster than classical algorithms.

- Uses **quantum period finding** and the **Quantum Fourier Transform**
- Employs classical pre- and post-processing for factor extraction
- Capable of factoring small numbers like 15 and 21 using simulators

---

## 🔍 Grover’s Algorithm – Quantum Search

Grover’s algorithm : find a marked item in an unsorted database with **quadratic speedup** over classical algorithms.

- Implements **Grover’s diffusion operator** and **oracle-based search**
- Visually shows the amplitude amplification through iterations
- Demonstrates success probability increasing with each iteration
