<h1 id="10b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $M_{\rm tot}=\sum_i m_i$ and introduce positions relative to the [centre of mass](../../../../../../center-of-mass.md), $\boldsymbol\rho_i=\boldsymbol r_i-\boldsymbol R$. The definition gives $\sum_i m_i\boldsymbol\rho_i=0$, and differentiation gives $\sum_i m_i\dot{\boldsymbol\rho}_i=0$. Expand the total [kinetic energy](../../../../../../kinetic-energy.md):

$$
\begin{aligned}
T&=\frac12\sum_i m_i|\dot{\boldsymbol R}+\dot{\boldsymbol\rho}_i|^2\\
&=\frac12M_{\rm tot}|\dot{\boldsymbol R}|^2
+\dot{\boldsymbol R}\cdot\sum_i m_i\dot{\boldsymbol\rho}_i
+\frac12\sum_i m_i|\dot{\boldsymbol\rho}_i|^2.
\end{aligned}
$$

The cross term vanishes. This proves the [kinetic energy decomposition about the center of mass](../../../../../../kinetic-energy-decomposition-about-the-center-of-mass.md):

$$
\boxed{T=T_1+T_2,\qquad
T_1=\frac12M_{\rm tot}|\dot{\boldsymbol R}|^2,\quad
T_2=\frac12\sum_i m_i|\dot{\boldsymbol\rho}_i|^2.}
$$

The decomposition itself holds without rigidity.

For a [rigid body](../../../../../../rigid-body-dynamics.md) rotating about its [centre of mass](../../../../../../center-of-mass.md), $\dot{\boldsymbol\rho}_i=\boldsymbol\omega\times\boldsymbol\rho_i$. With unit axis vector $\boldsymbol n=\boldsymbol\omega/|\boldsymbol\omega|$, the [moment of inertia](../../../../../../moment-of-inertia.md) about that axis is

$$
I=\sum_i m_i\left[|\boldsymbol\rho_i|^2-(\boldsymbol n\cdot\boldsymbol\rho_i)^2\right]
=\sum_i m_i d_i^2,
$$

where $d_i$ is the perpendicular distance from the axis. Therefore

$$
\boxed{T_2=\frac12 I\omega^2,\qquad \omega=|\boldsymbol\omega|.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10B](../../10b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
