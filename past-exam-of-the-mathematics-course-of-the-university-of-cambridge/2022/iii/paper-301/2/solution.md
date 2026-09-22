<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Suppose an infinitesimal continuous transformation has variations $\delta\psi,\delta\bar\psi$ and changes the Lagrangian density by $\delta\mathcal L=\partial_\mu K^\mu$. Expanding by the chain rule and integrating derivatives by parts gives

$$
\begin{aligned}
\delta\mathcal L
&=\left[\frac{\partial\mathcal L}{\partial\psi}
-\partial_\mu\frac{\partial\mathcal L}{\partial(\partial_\mu\psi)}\right]\delta\psi
+\left[\frac{\partial\mathcal L}{\partial\bar\psi}
-\partial_\mu\frac{\partial\mathcal L}{\partial(\partial_\mu\bar\psi)}\right]\delta\bar\psi\\
&\quad+\partial_\mu\left[
\frac{\partial\mathcal L}{\partial(\partial_\mu\psi)}\delta\psi
+\delta\bar\psi\frac{\partial\mathcal L}{\partial(\partial_\mu\bar\psi)}
\right].
\end{aligned}
$$

On solutions of the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md), the first two brackets vanish. Hence [Noether's theorem](../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md) gives the conserved current

$$
j^\mu
=\frac{\partial\mathcal L}{\partial(\partial_\mu\psi)}\delta\psi
+\delta\bar\psi\frac{\partial\mathcal L}{\partial(\partial_\mu\bar\psi)}-K^\mu,
\qquad \partial_\mu j^\mu=0.
$$

For spacetime transformations, the coordinate variation supplies the corresponding energy-momentum term.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
