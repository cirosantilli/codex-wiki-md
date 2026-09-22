<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [diffusion generator](../../../../diffusion-generator.md) is $\mathcal L=\mu\partial_x+\tfrac12\sigma^2\partial_{xx}$. By the [Feynman-Kac formula](../../../../feynman-kac-formula.md), the required [conditional characteristic function](../../../../conditional-characteristic-function.md) solves

$$
F_t+\mu F_x+\tfrac12\sigma^2F_{xx}=0,\qquad F(T,x)=e^{iux}.
$$

Use [separation of variables](../../../../separation-of-variables.md) in the form $F(t,x)=e^{iux}h(t)$. Since $F_x=iuF$ and $F_{xx}=-u^2F$, the temporal factor satisfies the [ordinary differential equation](../../../../ordinary-differential-equation.md)

$$
h'(t)+\left(iu\mu-\frac12\sigma^2u^2\right)h(t)=0,\qquad h(T)=1.
$$

Thus $h(t)=\exp[(iu\mu-\tfrac12\sigma^2u^2)(T-t)]$, and

$$
\boxed{\mathbb E[e^{iuX_T}\mid X_t=x]
=\exp\left(iu[x+\mu(T-t)]-\frac12u^2\sigma^2(T-t)\right).}
$$

This is bounded in absolute value by one, so it lies in the uniqueness class of the [Feynman-Kac formula](../../../../feynman-kac-formula.md). As an independent check, integrating the [stochastic differential equation](../../../../stochastic-differential-equation.md) gives $X_T=x+\mu(T-t)+\sigma(B_T-B_t)$. The independent [Brownian increments](../../../../brownian-increment.md) have the [normal distribution](../../../../normal-distribution.md) with mean zero and [variance](../../../../variance-split.md) $T-t$, yielding exactly the same [characteristic function](../../../../characteristic-function-split.md). For $\sigma=0$, the [conditional distribution](../../../../conditional-distribution.md) is a point mass at $x+\mu(T-t)$, and the same boxed expression still applies.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
