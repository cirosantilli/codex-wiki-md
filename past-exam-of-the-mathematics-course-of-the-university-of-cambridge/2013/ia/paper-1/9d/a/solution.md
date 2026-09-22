<h1 id="9d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonzero $x$, the absolute successive-term ratio in the exponential series is $|x|/(n+1)\to0$, so the first series converges for every $x$. For the factorial series the ratio is $(n+1)|x|\to\infty$, so its terms fail to tend to zero for every $x\ne0$.

The third series is sparse: its exponent is $n^2$, as in the PDF. If $t_n=(n!)^2|x|^{n^2}$, then

$$
\frac{t_{n+1}}{t_n}=(n+1)^2|x|^{2n+1}\longrightarrow0\qquad(0<|x|<1).
$$

For $|x|>1$, the terms grow without bound; at $|x|=1$ their moduli are $(n!)^2$, so they again fail the term test. Equivalently, the [Cauchy-Hadamard theorem](../../../../../../cauchy-hadamard-theorem.md) for the sparse coefficients uses $(n!)^{2/n^2}\to1$, not $(n!)^{2/n}\to\infty$. Thus the three [radii of convergence](../../../../../../radius-of-convergence.md) are

$$
\boxed{R_1=\infty,\qquad R_2=0,\qquad R_3=1.}
$$

Zeros at non-square coefficient indices do not change the relevant limsup in the last root test. This illustrates the [radius of convergence of a sparse power series](../../../../../../radius-of-convergence-of-a-sparse-power-series.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
