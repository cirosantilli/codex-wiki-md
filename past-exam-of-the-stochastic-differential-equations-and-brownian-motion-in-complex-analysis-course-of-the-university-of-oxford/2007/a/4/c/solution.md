<h1 id="a/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $G$ a standard [normal random variable](../../../../../gaussian-random-variable.md),

$$
\mathbb E f(X(t,x))
=\frac1{\sqrt{2\pi}}\int_{\mathbb R}
f(a(t)x+\sqrt{V(t)}\,z)e^{-z^2/2}dz.
$$

For $f\in C_b^1$, in the usual sense that $f$ and its continuous [derivative](../../../../../derivative.md) are bounded, the [mean value theorem](../../../../../mean-value-theorem.md) bounds the difference quotient by $a(t)\|f'\|_\infty$. [Dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore allows differentiation inside the [integral](../../../../../integral-split.md):

$$
\boxed{\frac d{dx}\mathbb E f(X(t,x))=a(t)\mathbb E f'(X(t,x))
=e^{\int_0^t\mu(s)ds}\mathbb E f'(X(t,x)).}
$$

This also follows pathwise from $X(t,x+h)-X(t,x)=a(t)h$. If the textual description were read as assuming only bounded differentiability, some control of $f'$ is needed for the displayed right side; the stated $C_b^1$ hypothesis supplies it. Gaussian smoothing itself still differentiates a bounded [measurable](../../../../../measurability.md) $f$, using the [derivative](../../../../../derivative.md) of the [Normal distribution](../../../../../normal-distribution.md) instead.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
