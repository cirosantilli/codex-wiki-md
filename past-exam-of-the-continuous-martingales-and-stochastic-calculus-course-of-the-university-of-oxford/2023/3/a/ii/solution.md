<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $X=(X^1,\ldots,X^d)$ be a [continuous semimartingale](../../../../../continuous-semimartingale.md), with $X^j=X_0^j+M^j+A^j$, where $M^j$ is a zero-starting [continuous local martingale](../../../../../continuous-local-martingale.md) and $A^j$ is a continuous [finite-variation process](../../../../../finite-variation-process.md) starting at zero. For $f\in C^{1,2}([0,\infty)\times\mathbb R^d)$, the [Itô formula](../../../../../ito-s-lemma.md) is

$$
\boxed{\begin{aligned}
f(t,X_t)=f(0,X_0)
&+\int_0^t\partial_sf(s,X_s)\,ds
+\sum_{j=1}^d\int_0^t\partial_jf(s,X_s)\,dX_s^j\\
&+\frac12\sum_{j,k=1}^d\int_0^t\partial_{jk}f(s,X_s)\,d[M^j,M^k]_s.
\end{aligned}}
$$

Here $[M^j,M^k]$ is the [quadratic covariation](../../../../../quadratic-covariation.md); the [finite-variation process](../../../../../finite-variation-process.md) parts contribute no such term. The integrals against the [finite-variation processes](../../../../../finite-variation-process.md) are understood pathwise, and those against the [continuous local martingales](../../../../../continuous-local-martingale.md) are [Itô integrals](../../../../../ito-integral.md) after localization.

For $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md) with [independent](../../../../../independent-random-variables.md) standard coordinates, $d[B^j,B^k]_s=\delta_{jk}ds$. In particular, if $f\in C^2$ is independent of time,

$$
f(B_t)=f(B_0)+\sum_j\int_0^t\partial_jf(B_s)\,dB_s^j
+\frac12\int_0^t\Delta f(B_s)\,ds,
$$

where $\Delta$ is the [Laplace operator](../../../../../laplace-operator.md). The same formulas hold up to exit from an open domain on which $f$ is smooth.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
