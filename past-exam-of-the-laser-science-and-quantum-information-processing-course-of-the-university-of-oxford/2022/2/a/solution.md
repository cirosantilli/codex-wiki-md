<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [complex beam parameter](../../../../complex-beam-parameter.md) convention

$$
\frac1q=\frac1{R_b}-i\frac{\lambda}{\pi w^2},\qquad q_{\rm waist}=iz_R.
$$

Here $R_b$ is the [wavefront](../../../../wavefront.md) curvature, distinguished from the mirror curvature $R$. In an unfolded propagation coordinate, a concave mirror has the [ray transfer matrix](../../../../ray-transfer-matrix-analysis.md) $\left(\begin{smallmatrix}1&0\\-2/R&1\end{smallmatrix}\right)$: a ray at height $x$ changes direction by $-2x/R$. The return to the original plane is therefore

$$
M=\begin{pmatrix}1&L\\0&1\end{pmatrix}
\begin{pmatrix}1&0\\-2/R&1\end{pmatrix}
\begin{pmatrix}1&L\\0&1\end{pmatrix}
=\begin{pmatrix}1-2L/R&2L(1-L/R)\\-2/R&1-2L/R\end{pmatrix}.
$$

The [Gaussian beam](../../../../gaussian-beam.md) transformation $q'=(Aq+B)/(Cq+D)$ gives

$$
\boxed{q'=\frac{(1-2L/R)iz_R+2L(1-L/R)}{1-2L/R-2iz_R/R}.}
$$

For $R=2L$, $M=\left(\begin{smallmatrix}0&L\\-1/L&0\end{smallmatrix}\right)$ and $q'=-L^2/q=iL^2/z_R$. The returning [Gaussian beam](../../../../gaussian-beam.md) consequently has a [beam waist](../../../../beam-waist.md) at the same plane, with

$$
\boxed{z_R'=L^2/z_R.}
$$

This alone does not make it the same [Gaussian beam](../../../../gaussian-beam.md); equal [Rayleigh ranges](../../../../rayleigh-length.md) require $z_R=L$.

Adding the plane mirror requires a self-consistent [optical resonator](../../../../optical-cavity.md) [normal mode](../../../../normal-mode.md), $q'=q=iz_R$. Since $A=D$, the fixed-point equation reduces to $Cq^2=B$, giving

$$
\boxed{z_R=\sqrt{L(R-L)}=\sqrt{LR(1-L/R)}.}
$$

For a finite stable [Gaussian beam](../../../../gaussian-beam.md), $0<L<R$. The same formula remains valid at $R=2L$, where self-consistency selects $z_R=L$. At the geometrical hemispherical limit $R=L$ it predicts $z_R=0$; that marginal boundary has no finite-width stable fundamental [Gaussian beam](../../../../gaussian-beam.md). Thus the source's word “hemispherical” is used for the plano-concave family, including the near-hemispherical case below.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
