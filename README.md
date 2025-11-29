# Discrete Fourier Transform and Signal Processing

**Course Project | Mathematics 703: Methods of Applied Mathematics**
**University of Wisconsin-Madison**

## 📄 Overview
This repository contains the research report and poster for a project investigating the mathematical foundations of the **Discrete Fourier Transform (DFT)** and its applications in **Sparse Signal Recovery**.

We explore how the **Uncertainty Principle** imposes limits on simultaneous time-frequency localization and demonstrate how these constraints can be leveraged to uniquely recover binary signals from incomplete frequency data using the **Direct Rounding Algorithm (DRA)**.

## 📂 Files
* **[`Report.pdf`](./Report.pdf)**: The detailed technical report containing definitions, complexity proofs for FFT, and derivations of the Donoho-Stark Uncertainty Principle.
* **[`Poster (PDF)`](./Discrete%20Fourier%20Transform%20and%20Signal%20Processing_poster.pdf)**: The visualization poster summarizing key theorems and the signal recovery framework.

## 🧮 Key Topics & Contributions

### 1. Fast Fourier Transform (FFT) Algorithms
* Analyzed the recursive structure of the FFT.
* Provided a rigorous proof that the complexity of calculating Fourier coefficients for a length-$N$ signal ($N=2^n$) is reduced from $O(N^2)$ (naive) to **$O(N \log N)$**.

### 2. Uncertainty Principles
* **Classical Uncertainty Principle:** Proved that for any nonzero signal, the product of its time support size ($N_t$) and frequency support size ($N_\omega$) satisfies $N_t N_\omega \ge N$.
* **Donoho-Stark Uncertainty Principle:** Investigated the condition for unique signal recovery, showing that a signal can be recovered despite missing frequencies if $N_t N_\omega < N/2$.

### 3. Sparse Signal Recovery
* Focus on **Binary Signals** (signals taking values in $\{0, 1\}$).
* Proved the validity of the **Direct Rounding Algorithm (DRA)**, which recovers a binary signal $E$ from a subset of observed frequencies, provided that the unobserved set $S$ satisfies $|E||S| < N/4$.

## 👥 Authors
* **Lejun Xu**
* Jiayi Hu
* Yi Jin
* Taylor Tan

## 📚 References
* E. M. Stein and R. Shakarchi, *Fourier Analysis: An Introduction*. Princeton University Press, 2003.
* D. L. Donoho and P. B. Stark, "Uncertainty principles and signal recovery," *SIAM Journal on Applied Mathematics*, 49:906-930, 1989.
