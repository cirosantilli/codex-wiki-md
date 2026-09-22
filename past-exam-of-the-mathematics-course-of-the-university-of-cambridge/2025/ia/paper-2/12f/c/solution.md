<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $u\mapsto(1+u/S)^{-n}$ decreases, $X_i<X_{i+1}$ exactly when $E_i>E_{i+1}$. Therefore $K\ge i$ exactly when $E_1\le\cdots\le E_i$, an event of probability $1/i!$ independent of $S$. The tail-sum rearrangement gives

$$
\mathbb E\sum_{i=1}^KS^i=\sum_{i=1}^n\mathbb E[S^i]\mathbb P(K\ge i).
$$

Since $\mathbb E[S^i]=(n+i-1)!/(n-1)!$, the $i$th term is $\binom{n+i-1}{i}$, proving the formula.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
