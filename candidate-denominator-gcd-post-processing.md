# Candidate-denominator gcd post-processing

↑ **Parent:** [Shor's algorithm](shor-s-algorithm.md)

After [continued-fraction recovery in quantum order finding](continued-fraction-recovery-in-quantum-order-finding.md), an even candidate denominator $q$ can be used to try the displayed [greatest common divisors](greatest-common-divisor.md). Return only a divisor strictly between one and $N$. If $q$ is the true even [multiplicative order](multiplicative-order.md) with a nontrivial halfway power, success follows from [factor extraction from an even modular order](factor-extraction-from-an-even-modular-order.md). A candidate that is not a period can occasionally still yield a factor; testing $a^q\equiv1$ before the gcds therefore changes single-run success probabilities. The output-factor check guarantees correctness in either convention.

## ↑ Ancestors (5)

1. [Shor's algorithm](shor-s-algorithm.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/1/iii/solution.md)
