# The Ash Kelly Prime Number Solver

## Overview
The **Ash Kelly Prime Number Solver** is an advanced deterministic prime number predictor that estimates the nth prime number with high accuracy. This algorithm leverages harmonic corrections, empirical adjustments, and nonlinear phase shift refinements to improve precision beyond classical approximations like the Prime Number Theorem.

This project is **MIT licensed** and is being released as an **open-source** contribution. The **primary author is Ash Kelly**, with additional refinements and optimizations integrated into this version.

## Features
- **Empirical Correction Constant:** A dynamically tuned correction function enhances accuracy.
- **Harmonic Frequencies:** Uses selected harmonic frequencies to fine-tune estimates.
- **Dynamic Harmonic Weighting:** Introduces a logarithmically scaled weight to balance corrections.
- **Nonlinear Phase Shift Correction:** A cosine-based adjustment improves results.
- **Prime Validation:** Ensures the estimated prime is correct by locally refining the prediction using sympy’s prime functions.

## Installation
Ensure you have Python installed (version 3.x recommended). Install dependencies using:
```bash
pip install numpy sympy
```

## Usage
The script provides an implementation of the `universal_prime_function(n)`, which predicts the nth prime number. Example usage:

```python
from prime_solver import universal_prime_function

n = 1000  # Example: Find the 1000th prime number
predicted_prime = universal_prime_function(n)
print(f"Predicted {n}th prime: {predicted_prime}")
```

Alternatively, you can run the script directly:
```bash
python prime_solver.py
```

## Example Output
Running the script with predefined test cases prints:
```plaintext
Predicted 100th prime: 541, Actual: 541, Error: 0
Predicted 500th prime: 3571, Actual: 3571, Error: 0
Predicted 1000th prime: 7919, Actual: 7919, Error: 0
Predicted 5000th prime: 48611, Actual: 48611, Error: 0
Predicted 10000th prime: 104729, Actual: 104729, Error: 0
```

## How It Works
The function estimates the nth prime number using:
1. **Base Approximation**: Derived from classical prime number theorems.
2. **Empirical Correction**: Refines the estimate dynamically based on `n`.
3. **Harmonic Adjustments**: Applies small oscillatory corrections to enhance accuracy.
4. **Final Refinement**: Uses sympy to ensure the output is a prime number.

## License
This project is released under the **MIT License**, allowing free and open usage.

## Acknowledgments
- **Primary Author:** Ash Kelly
- **Additional Contributors:** Richard Aragon
- **Libraries Used:** `numpy`, `sympy`

## Contributions
Contributions are welcome! Feel free to submit pull requests or open issues to enhance the algorithm further.

## Contact
For questions or collaboration, please reach out via the GitHub issues section.

---
Happy Prime Hunting! 🎯

