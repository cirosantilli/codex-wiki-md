# Full-period criterion for a mixed congruential generator

↑ **Parent:** [Linear congruential generator](linear-congruential-generator.md)

A [linear congruential generator](linear-congruential-generator.md) has period $M$ for every seed if and only if $\gcd(c,M)=1$, every prime dividing $M$ divides $a-1$, and $4\mid M$ implies $4\mid a-1$. The coprimality of $c$ prevents the orbit from being trapped in a residue class; the multiplier conditions permit full-period lifting through each prime power. Combining the prime-power periods by the [Chinese remainder theorem](chinese-remainder-theorem.md) gives period $M$. For $M=12^k=2^{2k}3^k$, the multiplier criterion reduces to $a\equiv1\pmod{12}$, together with $\gcd(c,6)=1$. A positive increment alone is insufficient.

## ↑ Ancestors (7)

1. [Linear congruential generator](linear-congruential-generator.md)
2. [Pseudorandom number generator](pseudorandom-number-generator.md)
3. [Monte Carlo method](monte-carlo-method.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/3/a/solution.md)
