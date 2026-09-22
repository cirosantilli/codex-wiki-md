<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At the cusp of $f_0(t)=|t|$, positivity and evenness of the [Fejér kernel](../../../../../../fejer-kernel.md) give

$$
\sigma_n(f_0,0)-f_0(0)
=\frac2\pi\int_0^\pi F_n(t)t\,dt.
$$

Since $\sin(t/2)\leq t/2$,

$$
\sigma_n(f_0,0)
\geq\frac4{\pi n}\int_0^\pi
\frac{\sin^2(nt/2)}{t}\,dt.
$$

Summing the supplied lower bound over $I_k$, $1\leq k\leq n'=\lfloor n/2\rfloor$, yields

$$
\sigma_n(f_0,0)
\geq\frac{c}{n}\sum_{k=1}^{n'}\frac1k.
$$

The [harmonic series](../../../../../../harmonic-series.md) satisfies $\sum_{k=1}^{n'}k^{-1}\geq c'\log n$, so

$$
\boxed{|\sigma_n(f_0,0)-f_0(0)|
\geq c_1'\frac{\log n}{n}}.
$$

The [modulus of continuity](../../../../../../modulus-of-continuity.md) of the periodic function $f_0$ obeys $\omega(f_0,1/n)=1/n$. If a universal [Jackson-type estimate](../../../../../../jackson-type-estimate.md)

$$
\|\sigma_n(f)-f\|_\infty\leq C\omega(f,1/n)
$$

held for all continuous periodic $f$, it would give $O(1/n)$ for $f_0$, contradicting the lower bound. Thus

$$
\boxed{\text{no such universal Jackson-type estimate holds for Fejér sums}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
