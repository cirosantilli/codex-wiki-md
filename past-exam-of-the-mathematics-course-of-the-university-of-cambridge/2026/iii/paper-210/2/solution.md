<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [kernel for density estimation](../../../../../kernel-for-density-estimation.md) is a bounded nonnegative integrable function $K$ with $\int_{\mathbb R}K=1$. Its bandwidth-$h$ rescaling is $K_h(u)=h^{-1}K(u/h)$, and the [kernel density estimator](../../../../../kernel-density-estimation.md) is

$$
\widehat f_n(x)=\frac1n\sum_{i=1}^nK_h(x-X_i).
$$

Fix $x$ and put $V_i=K_h(x-X_i)$. Since $K$ vanishes outside $[-1,1]$,

$$
\mathbb EV_1^2
\leq\frac{\lVert K\rVert_\infty^2}{h^2}
\int_{x-h}^{x+h}f(y)\,dy
=\frac{2\lVert K\rVert_\infty^2}{h}f_h(x).
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and [variance additivity for independent random variables](../../../../../variance-additivity-for-independent-random-variables.md) give

$$
\mathbb E|\widehat f_n(x)-\mathbb E\widehat f_n(x)|
\leq\lVert K\rVert_\infty
\frac{2^{1/2}f_h(x)^{1/2}}{(nh)^{1/2}}.
$$

Nonnegativity also gives $\mathbb E|V_1-\mathbb EV_1|\leq2\mathbb EV_1\leq4\lVert K\rVert_\infty f_h(x)$. Taking the better estimate at each $x$ and applying [Tonelli theorem](../../../../../tonelli-theorem.md) proves

$$
\mathbb E\int_{-\infty}^{\infty}|\widehat f_n-\mathbb E\widehat f_n|
\leq\lVert K\rVert_\infty\int_{-\infty}^{\infty}
\min\left\{
\frac{2^{1/2}f_h^{1/2}}{(nh)^{1/2}},4f_h
\right\}.
$$

For nonnegative $a,b$ and $0\leq\theta\leq1$, $\min{a,b}\leq a^\theta b^{1-\theta}$. Taking $\theta=2\rho$ yields

$$
\mathbb E\int|\widehat f_n-\mathbb E\widehat f_n|
\leq\frac{2^{2-3\rho}\lVert K\rVert_\infty}{(nh)^\rho}
\int f_h^{1-\rho}.
$$

For $\rho>0$, the [Holder inequality](../../../../../holder-inequality.md) with conjugate exponents $(1-\rho)^{-1}$ and $\rho^{-1}$ gives

$$
\int f_h^{1-\rho}
\leq C_{\rho,\delta}^{\rho}
\left(\int(1+|x|)^\delta f_h(x)\,dx\right)^{1-\rho}.
$$

If $U$ is uniform on $[-1,1]$ and independent of $X_1$, then $X_1+hU$ has [probability density function](../../../../../probability-density-function.md) $f_h$. Since

$$
1+|X_1+hU|\leq(1+h)(1+|X_1|),
$$

the last integral is at most $(1+h)^\delta\int(1+|x|)^\delta f(x)\,dx$. Substitution proves the second displayed bound. The case $\rho=0$ is the first bound integrated using $\int f_h=1$ and follows directly.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
