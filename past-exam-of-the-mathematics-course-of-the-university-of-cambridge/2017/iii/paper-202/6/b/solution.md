<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the true [martingale](../../../../../../martingale-split.md) of part (a), $M_0=u(T,x)$ and $M_T=f(B_T)e^{A_T}$. Taking [expectations](../../../../../../expected-value.md) gives the [Feynman-Kac formula with a bounded potential](../../../../../../feynman-kac-formula-with-a-bounded-potential.md):

$$
\boxed{u(t,x)=\mathbb E_x\left[f(B_t)\exp\!\left(\int_0^t\frac{ds}{1+B_s^2}\right)\right].}
$$

The right side is finite since its absolute value is at most $e^t\|f\|_\infty$. This also proves uniqueness among [classical solutions](../../../../../../classical-solution.md) bounded on every finite time slab: applying the formula to their difference with zero initial data gives zero. The positive sign of the potential in the [partial differential equation](../../../../../../partial-differential-equation-split.md) explains the positive exponent; changing it to a negative exponent would solve a different equation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
