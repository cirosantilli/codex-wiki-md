# Linear congruential generator

↑ **Parent:** [Pseudorandom number generator](pseudorandom-number-generator.md)

Choose integers $M>1$, $a$, $c$ and a seed $S_0$. Iterate $S_{n+1}=(aS_n+c)\bmod M$ and return $U_n=S_n/M$. This gives a deterministic finite-state [pseudorandom number generator](pseudorandom-number-generator.md) with output in $[0,1)$. A nonzero increment gives a mixed generator; $c=0$ gives a multiplicative generator. Its period is at most $M$, but even a full period does not guarantee good multidimensional uniformity or statistical [independence](independent-random-variables.md).

**Table of contents**

- [Full-period criterion for a mixed congruential generator](full-period-criterion-for-a-mixed-congruential-generator.md)

## ↑ Ancestors (6)

1. [Pseudorandom number generator](pseudorandom-number-generator.md)
2. [Monte Carlo method](monte-carlo-method.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Full-period criterion for a mixed congruential generator](full-period-criterion-for-a-mixed-congruential-generator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/3/a/solution.md)
- [Pseudorandom number](pseudorandom-number.md)
