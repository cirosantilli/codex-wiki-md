<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Schoenberg spline operator](../../../../../../schoenberg-spline-operator.md) is positive and $V_n1=1$. If $\xi_i=a_{1,i}$, then both $\tau_i$ and $\xi_i$ lie in $[t_i,t_{i+k}]$, so

$$
\lVert V_nt-t\rVert_\infty\leq k|\Delta_n|\to0.
$$

Because $a_{2,i}$ averages products of knots in the same interval and all points lie in $[0,1]$,

$$
\lVert V_nt^2-t^2\rVert_\infty\leq2k|\Delta_n|\to0.
$$

The [Korovkin theorem](../../../../../../korovkin-theorem.md) now proves

$$
\boxed{\lVert V_n(f)-f\rVert_{C[0,1]}\to0}
$$

for every $f\in C[0,1]$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
