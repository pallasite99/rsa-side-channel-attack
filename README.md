# RSA Timing Attack Demonstration & Countermeasures

## Overview
This project demonstrates a **side-channel timing attack** on RSA decryption and explores countermeasures using **constant-time exponentiation**. The attack exploits variations in decryption time to infer bits of the private key.

## Features
- Implements **RSA encryption and decryption**.
- Simulates a **timing attack** using naive modular exponentiation.
- Introduces **constant-time exponentiation** to mitigate the attack.
- Compares **timing variations** using statistical analysis.
- Visualizes timing data with **histograms**.

## Installation
Ensure you have Python 3 installed. Install dependencies using:

```sh
pip install numpy matplotlib pycryptodome
```

## Usage
Run the script to:
1. Generate an RSA key pair.
2. Encrypt and decrypt a sample message.
3. Perform a timing attack on the naive decryption.
4. Apply constant-time exponentiation.
5. Compare and visualize results.

```sh
python rsa_timing_attack.py
```

## Results
- The naive RSA implementation shows **timing variations**, making it vulnerable.
- The constant-time implementation eliminates these variations, **preventing key leakage**.
- Histogram plots illustrate the **effectiveness of mitigation**.

## Example Output

```
Average decryption time (Naive): 0.000456 seconds, Std Dev: 0.000034
Decryption time (Constant-Time): 0.000422 seconds
Timing attack effectiveness reduced with constant-time exponentiation!
```

## Visualization
The script generates a histogram comparing decryption times:

![Timing Attack Histogram](example_plot.png)

## References
- Paul C. Kocher, "Timing Attacks on Implementations of Diffie-Hellman, RSA, DSS, and Other Systems"
- Cryptography Engineering by Niels Ferguson, Bruce Schneier, and Tadayoshi Kohno

## License
This project is licensed under the MIT License.

---
Contributions and improvements are welcome! 🚀

