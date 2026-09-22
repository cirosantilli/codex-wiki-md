<h1 id="12e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [continuous approximation of a Riemann-integrable function](../../../../../../continuous-approximation-of-a-riemann-integrable-function.md) follows here by choosing partitions $P_n$ with upper-minus-lower sum below $1/n$. On each subinterval choose the midpoint of the infimum and supremum to form a step [function](../../../../../../function-split.md) $s_n$. Then

$$
\int_a^b|g-s_n|<\frac1n.
$$

Replace each of the finitely many jumps of $s_n$ by a linear transition on intervals of sufficiently small total length, obtaining a continuous $\phi_n$ with $\int|s_n-\phi_n|<1/n$. Hence $\int|g-\phi_n|<2/n$, and uniformly for every subinterval $[\alpha,\beta]$,

$$
\boxed{\left|\int_\alpha^\beta(g-\phi_n)\right|\leq\int_a^b|g-\phi_n|\to0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12E](../../12e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
