<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [path integral](../../../../../path-integral.md) with source term

$$
S_{\mathrm{src}}=\int d^4x\,[J^\mu A_\mu+\bar\eta_\alpha\psi_\alpha+\bar\psi_\alpha\eta_\alpha].
$$

The sources $\eta,\bar\eta$ are [Grassmann variables](../../../../../grassmann-variable.md); all derivatives below are left [functional derivatives](../../../../../functional-derivative.md). Because $\eta$ stands to the right of $\bar\psi$, differentiating with respect to it introduces a minus sign. The insertion rules are therefore

$$
\frac1i\frac{\delta}{\delta J^\mu}\longleftrightarrow A_\mu,\qquad
i\frac{\delta}{\delta\eta_\alpha}\longleftrightarrow\bar\psi_\alpha,\qquad
\frac1i\frac{\delta}{\delta\bar\eta_\beta}\longleftrightarrow\psi_\beta.
$$

For example $\delta_L(\bar\psi\eta)/\delta\eta=-\bar\psi$. The order of the odd [functional derivatives](../../../../../functional-derivative.md) matters: the rightmost derivative acts first, and the displayed product inserts $\bar\psi_\alpha\psi_\beta$ in that order.

Expand $\exp[-ie\int\bar\psi\gamma^\mu\psi A_\mu]$ in its [power series](../../../../../power-series.md), replace each field by its source derivative, and pull the derivatives outside the free [path integral](../../../../../path-integral.md). Re-exponentiating gives

$$
\boxed{Z[J,\eta,\bar\eta]=\exp\left[-ie\int d^4x\left(\frac1i\frac{\delta}{\delta J^\mu(x)}\right)\left(i\frac{\delta}{\delta\eta_\alpha(x)}\right)\gamma^\mu_{\alpha\beta}\left(\frac1i\frac{\delta}{\delta\bar\eta_\beta(x)}\right)\right]Z_0[J,\eta,\bar\eta].}
$$

This identity concerns the unnormalized [generating functional](../../../../../generating-functional.md). Normalized [correlation functions](../../../../../correlation-function.md) divide by its zero-source value so that vacuum contributions cancel.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2020](../../../../2020-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
