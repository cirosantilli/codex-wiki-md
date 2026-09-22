<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret $H_{-\infty}(\mathbb T^n)=\bigcup_{s\in\mathbb R}H^s(\mathbb T^n)$, the periodic [distributions](../../../../../../distribution-mathematical-analysis.md) of finite negative [Sobolev space](../../../../../../sobolev-space-split.md) order. Smooth multiplication is bounded on every [periodic Sobolev space](../../../../../../periodic-sobolev-space.md). One direct proof uses the rapid decay of the [Fourier coefficients](../../../../../../fourier-coefficient.md) of $V$: the inequality

$$
\langle k\rangle^s\leq C_s\langle k-\ell\rangle^{|s|}\langle\ell\rangle^s,\qquad\langle k\rangle=(1+|k|^2)^{1/2},
$$

reduces the weighted convolution formula for $\widehat{Vf}$ to an $\ell^1*\ell^2$ estimate. Thus $\|Vf\|_{H^s}\leq C_{V,s}\|f\|_{H^s}$ for every real $s$.

Suppose initially $f\in H^s$. The equation gives $\Delta f=u-Vf\in H^s$, since a [smooth function](../../../../../../smooth-function.md) belongs to every [periodic Sobolev space](../../../../../../periodic-sobolev-space.md). For $k\ne0$, the [Fourier multiplier](../../../../../../fourier-multiplier.md) of $\Delta$ is $|k|^2$, and

$$
(1+|k|^2)^{s+2}|\widehat f(k)|^2
\leq4(1+|k|^2)^s|\widehat{\Delta f}(k)|^2.
$$

The zero coefficient is already finite. Hence $f\in H^{s+2}$. Iterating the argument gives $f\in H^{s+2j}$ for every $j\geq0$. Applying the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) also to each distributional [partial derivative](../../../../../../partial-derivative.md) produces a smooth representative. Therefore $\boxed{f\in C^\infty(\mathbb T^n)}$. This is an explicit [elliptic regularity bootstrap](../../../../../../elliptic-regularity-bootstrap-with-smooth-lower-order-coefficients.md), valid for complex or real $V$ and without a sign assumption on it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
