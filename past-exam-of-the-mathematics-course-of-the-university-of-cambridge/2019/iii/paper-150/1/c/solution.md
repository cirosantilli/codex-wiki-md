<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The same divisor-identity argument as in part (a) gives

$$
\sum_{n\leq x}\frac{\Lambda(n)}n=\log x+O(1).
$$

On the other hand, the [Abel summation formula](../../../../../../abel-s-summation-formula.md) gives

$$
\sum_{n\leq x}\frac{\Lambda(n)}n
=\frac{\psi(x)}x+\int_1^x\frac{\psi(t)}{t^2}\,dt.
$$

Under the proposed asymptotic, the right side is

$$
a\log x+b\log\log x+o(\log\log x)+O(1).
$$

Dividing first by $\log x$ gives $a=1$. Subtracting $\log x$, dividing by $\log\log x$, and taking the [limit](../../../../../../limit-of-a-function.md) then gives $b=0$. Therefore

$$
\boxed{a=1,\qquad b=0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
