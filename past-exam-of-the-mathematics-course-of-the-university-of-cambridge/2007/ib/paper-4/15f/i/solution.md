<h1 id="15f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an integer $n\ge0$ and $\operatorname{Re}s>0$, the definition of the [Laplace transform](../../../../../../laplace-transform.md) gives $F_0(s)=\int_0^\infty e^{-st}\,dt=1/s$. For $n\ge1$, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
F_n(s)=\left[-\frac{t^ne^{-st}}s\right]_0^\infty+\frac ns\int_0^\infty t^{n-1}e^{-st}\,dt=\frac nsF_{n-1}(s).
$$

The endpoint term vanishes because [exponential decay](../../../../../../exponential-decay.md) dominates every fixed power of $t$. Induction therefore gives $F_n(s)=n!/s^{n+1}$. Multiplication by $e^{at}$ replaces $e^{-st}$ by $e^{-(s-a)t}$ in the defining [integral](../../../../../../integral.md), so

$$
\boxed{\mathcal L(t^n)(s)=\frac{n!}{s^{n+1}},\qquad\mathcal L(e^{at}t^n)(s)=\frac{n!}{(s-a)^{n+1}}.}
$$

The second formula holds for $\operatorname{Re}(s-a)>0$ and is the [Laplace transform shift theorem](../../../../../../laplace-transform-shift-theorem.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [15F](../../15f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
