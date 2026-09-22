<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $v_k=p_k(1-p_k)$ and assume $0<p_k<1$. For fixed $n$ and a fixed nonzero difference $\Delta=p_0-p_1$, the approximate [statistical power](../../../../../../statistical-power.md) of the [Wald test](../../../../../../wald-test.md) increases as its noncentrality $|\Delta|/\sqrt V$ increases, where

$$
V=\frac{v_0}{n_0}+\frac{v_1}{n-n_0}.
$$

Differentiating with respect to the continuous allocation gives

$$
\frac{dV}{dn_0}=-\frac{v_0}{n_0^2}+\frac{v_1}{n_1^2}=0,\qquad
\frac{d^2V}{dn_0^2}=\frac{2v_0}{n_0^3}+\frac{2v_1}{n_1^3}>0.
$$

Hence the unique minimum and its associated minimum [variance](../../../../../../variance-split.md) are

$$
\boxed{R^*=\frac{n_0}{n_1}=\sqrt{\frac{p_0(1-p_0)}{p_1(1-p_1)}},\qquad
V_{\min}=\frac{(\sqrt{v_0}+\sqrt{v_1})^2}{n}.}
$$

This is [Neyman allocation](../../../../../../neyman-allocation.md). Integer allocations use a feasible adjacent integer to the continuous optimum, comparing the resulting [variances](../../../../../../variance-split.md); $n_0,n_1\geq1$ must still hold. It is a large-sample [normal approximation](../../../../../../normal-approximation.md) argument, not an exact finite-sample power theorem for arbitrary [response-adaptive randomization](../../../../../../response-adaptive-randomization.md). Under the null $p_0=p_1$, the approximate power is the [significance level](../../../../../../significance-level.md) for any allocation, although the same allocation still minimizes the stated [variance](../../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
