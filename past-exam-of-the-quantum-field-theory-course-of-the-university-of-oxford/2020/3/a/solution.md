<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Keep $\lambda$ for the cubic coupling and $j$ for the external [source](../../../../source-quantum-field-theory.md). Expanding the interaction part of the [scalar field path integral](../../../../scalar-field-path-integral.md) yields

$$
Z[\lambda;j]=\sum_{V=0}^\infty\frac1{V!}
\left(-\frac{i\lambda}{3!}\right)^V
\int\prod_{v=1}^V d^4y_v\int D\phi\,
\prod_{v=1}^V\phi(y_v)^3\,
 e^{iS_0[\phi]+i\int j\phi}.
$$

A [functional derivative](../../../../functional-derivative.md) of the source exponential inserts $i\phi(y)$. In particular, $\delta_j(y)^3 e^{i\int j\phi}=-i\phi(y)^3e^{i\int j\phi}$, so $-i\lambda\phi(y)^3$ can be replaced by $\lambda\delta_j(y)^3$. The [functional derivatives](../../../../functional-derivative.md) commute and can be taken outside the free [path integral](../../../../path-integral.md). Resumming the [exponential series](../../../../exponential-series.md) gives

$$
\boxed{Z[\lambda;j]=\exp\left[\frac\lambda{3!}\int d^4y\,
\frac{\delta^3}{\delta j(y)^3}\right]Z[0;j].}
$$

This is a formal [perturbation series](../../../../perturbation-series.md); a real cubic [scalar potential](../../../../scalar-potential.md) is unbounded and the expression does not assert a stable nonperturbative [vacuum state](../../../../vacuum-state.md).

To evaluate the free [Gaussian path integral](../../../../gaussian-path-integral.md), use [integration by parts](../../../../integration-by-parts.md) to write

$$
S_0[\phi]+\int j\phi=\frac12\int\phi K\phi+\int j\phi,
\qquad K=-\Box-m^2+i\epsilon.
$$

The inverse kernel is

$$
K^{-1}(x,y)=D(x-y)
=\int\frac{d^4p}{(2\pi)^4}
\frac{e^{-ip\cdot(x-y)}}{p^2-m^2+i\epsilon}.
$$

[Completing the square](../../../../completing-the-square.md) with $\phi=\chi-K^{-1}j$ changes the exponent to $i\int\chi K\chi/2-i\int jK^{-1}j/2$. The translation-invariant [functional measure](../../../../functional-measure.md) makes the remaining [Gaussian path integral](../../../../gaussian-path-integral.md) precisely $Z[0;0]$, hence

$$
\boxed{Z[0;j]=Z[0;0]\exp\left[-\frac i2\int d^4x\,d^4y
\int\frac{d^4p}{(2\pi)^4}
\frac{j(x)j(y)e^{-ip\cdot(x-y)}}{p^2-m^2+i\epsilon}\right].}
$$

For $\epsilon>0$, the exponent includes $-\epsilon\int\phi^2/2$, which damps the regulated finite-dimensional integrals. The [Feynman i-epsilon prescription](../../../../feynman-i-epsilon-prescription.md) displaces the positive-[energy](../../../../energy-split.md) pole below the real $p^0$ axis and the negative-[energy](../../../../energy-split.md) pole above it, selecting the time-ordered [vacuum expectation value](../../../../vacuum-expectation-value.md). Indeed the [Feynman propagator](../../../../feynman-propagator.md) is $\Delta_F=iD$. Thus $i\epsilon$ specifies both convergence and the [vacuum state](../../../../vacuum-state.md) boundary conditions, with $\epsilon\to0^+$ taken after integration.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
