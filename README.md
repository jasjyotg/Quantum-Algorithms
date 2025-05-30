# Shor’s Algorithm – Quantum Factorization

This notebook implements **Shor’s Algorithm** using Qiskit, demonstrating how quantum computing can factor composite numbers exponentially faster than classical algorithms.

---



###  1. Problem Setup  
- Chose a **composite number N** (e.g., 15) to factor.
- Randomly selected an integer `a` such that `gcd(a, N) = 1`.

###  2. Classical Preprocessing  
- Checked if `a` is already a factor using the GCD.
- Handled special cases like even numbers or perfect powers before running quantum routines.

### 3. Quantum Circuit for Period Finding  
- Constructed a **quantum circuit** to find the period `r` of the function \( f(x) = a^x \mod N \).
- Used Qiskit's Aer simulator.
- Applied **modular exponentiation** in a quantum subroutine.
- Performed **Inverse Quantum Fourier Transform** (manually implemented).

###  4. Post-Processing: Extracting Factors  
- Used continued fractions to estimate the period `r` from measurements.
- Checked if:
  - \( r \) is even
  - \( a^{r/2} \not\equiv -1 \mod N \)
- Calculated factors using:
  \[
  \gcd(a^{r/2} \pm 1, N)
  \]

###  5. Loop Until Success  
- Repeated the entire algorithm with new values of `a` until successful.
- Printed results and tracked how many attempts were made.

---

## 📷 Example Output

