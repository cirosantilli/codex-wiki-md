<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $R_\varepsilon=\int_0^\varepsilon(H_u-H_0)\,dB_u$ and $d_\varepsilon=\varepsilon^{-1}\int_0^\varepsilon\mathbb E|H_u-H_0|^2du$. Boundedness and path continuity of $H$ make $\mathbb E|H_u-H_0|^2\to0$ by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), so $d_\varepsilon\to0$. The [Itô isometry](../../../../../../ito-isometry.md) gives $\mathbb E R_\varepsilon^2=\varepsilon d_\varepsilon$.

We must not assume independence between the integral and its Brownian denominator. Instead, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\mathbb E\left|\frac{R_\varepsilon}{B_\varepsilon}\right|^{1/4}
\leq\bigl(\mathbb E|R_\varepsilon|^{1/2}\bigr)^{1/2}\bigl(\mathbb E|B_\varepsilon|^{-1/2}\bigr)^{1/2}.
$$

Concavity, or [Jensen inequality](../../../../../../jensen-s-inequality.md), bounds the first factor by $(\mathbb E R_\varepsilon^2)^{1/8}$. Since $B_\varepsilon\overset d=\sqrt\varepsilon N$, the second factor is $\varepsilon^{-1/8}(\mathbb E|N|^{-1/2})^{1/2}$. This negative normal moment is finite: the density is bounded near zero, where $\int_0^1u^{-1/2}du<\infty$, and has Gaussian decay at infinity. In fact $\mathbb E|N|^{-1/2}=2^{-1/4}\Gamma(1/4)/\sqrt\pi$. The powers of $\varepsilon$ cancel, yielding the [fractional-moment control of Brownian increment ratios](../../../../../../fractional-moment-control-of-brownian-increment-ratios.md)

$$
\boxed{\mathbb E\left|\frac{R_\varepsilon}{B_\varepsilon}\right|^{1/4}\leq C d_\varepsilon^{1/8}\longrightarrow0,\qquad C=(\mathbb E|N|^{-1/2})^{1/2}.}
$$

The ratio may be assigned any value on the null event $B_\varepsilon=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
