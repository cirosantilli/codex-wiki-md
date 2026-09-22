<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Every word in $C_n(r)$ has probability at least $2^{-nr}$, so normalization gives $|C_n(r)|\leq2^{nr}$. Choose $H(U)<r<R$ and then $\varepsilon<r-H(U)$. Every $\varepsilon$-typical word satisfies $p(u^n)\geq2^{-n(H(U)+\varepsilon)}\geq2^{-nr}$, hence $T_\varepsilon^{(n)}\subseteq C_n(r)$ and $\Pr[C_n(r)]\to1$. Injectively encoding $C_n(r)$ and using a default codeword outside it gives rate at most $R$ and vanishing error.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
