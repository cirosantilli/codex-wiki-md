<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

A [normal mode](../../../../../normal-mode.md) is a [small oscillation](../../../../../small-oscillation.md) with fixed relative displacement amplitudes, all coordinates oscillating at one [frequency](../../../../../frequency.md). [linearization](../../../../../linearization.md) gives $M\ddot{\mathbf y}=-K\mathbf y$, so mode shapes solve $K\mathbf u=\omega_n^2M\mathbf u$.

Write $C=q^2/(4\pi\epsilon_0)$. [force](../../../../../force-split.md) balance on an outer ion gives $m\omega^2x_0=C/x_0^2+C/(2x_0)^2$, hence

$$
\boxed{x_0=\left(\frac{5q^2}{16\pi\epsilon_0m\omega^2}\right)^{1/3}.}
$$

A pair separated by $d$ has quadratic [energy](../../../../../energy-split.md) $C(y_j-y_i)^2/d^3$, equivalent to spring constant $2C/d^3$. The adjacent-pair constants are $8m\omega^2/5$, and the outer-pair constant is $m\omega^2/5$. Adding the trap stiffness gives

$$
\ddot{\mathbf y}=-\frac{\omega^2}{5}
\begin{pmatrix}14&-8&-1\\-8&21&-8\\-1&-8&14\end{pmatrix}\mathbf y.
$$

In the [three-ion axial normal modes](../../../../../three-ion-axial-normal-modes.md), the translation mode leaves every separation unchanged. The antisymmetric breathing mode leaves the central ion fixed; the remaining vector is [orthogonal](../../../../../orthogonal-vectors.md) to both. Direct multiplication yields

$$
\boxed{\begin{array}{c|c}
\text{mode vector}&\text{angular frequency}\\\hline
(1,1,1)&\omega\\
(1,0,-1)&\sqrt3\omega\\
(1,-2,1)&\sqrt{29/5}\,\omega
\end{array}}
$$

For [breathing excitation after a trap-frequency quench](../../../../../breathing-excitation-after-a-trap-frequency-quench.md), put $\omega'=\omega+\delta\omega$ and $x_0'=x_0(\omega/\omega')^{2/3}$. The displacement from the new equilibrium is solely along the breathing vector and the initial [velocity](../../../../../velocity.md) is zero. To first order in the fractional quench,

$$
\boxed{x_2(t)=0,\qquad x_{1,3}(t)=\mp\left[x_0'+(x_0-x_0')\cos(\sqrt3\omega't)\right],
\quad x_0-x_0'\simeq\frac{2x_0\delta\omega}{3\omega}.}
$$

The [frequency](../../../../../frequency.md) shown is the linearized [frequency](../../../../../frequency.md) about the new equilibrium. Nonlinear amplitude corrections are beyond this small-quench result.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
