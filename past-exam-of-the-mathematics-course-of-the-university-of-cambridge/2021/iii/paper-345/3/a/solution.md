<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Batchelor entrainment](../../../../../../batchelor-entrainment-hypothesis.md) models a turbulent plume as drawing ambient fluid inward at a speed proportional to its characteristic vertical velocity. In a top-hat axisymmetric plume, let

$$
Q=\pi b^2w,\qquad
M=\pi b^2w^2,\qquad
F=Qg'
$$

be volume, momentum, and buoyancy flux. The Boussinesq approximation uses a common density in inertia and volume conservation while retaining the small density difference in $g'=g(\rho_0-\rho)/\rho_0$. It requires $g'\ll g$ and becomes inaccurate for very hot source fluid or near openings with large density changes.

For a point source in an unstratified lower layer, the integral plume equations are

$$
\frac{dQ}{dz}=E\sqrt M,\qquad
\frac{dM}{dz}=\frac{FQ}{M},\qquad
\frac{dF}{dz}=0,
\qquad E=2\alpha\sqrt\pi,
$$

where $\alpha$ is the entrainment coefficient. Their pure-plume solution is

$$
\boxed{
Q_1(z)=C_QF_1^{1/3}z^{5/3},
\qquad
M_1(z)=C_MF_1^{2/3}z^{4/3},
\qquad
g'_{10}(z)=\frac{F_1}{Q_1(z)}
},
$$

with

$$
C_M=\left(\frac{9E}{20}\right)^{2/3},
\qquad
C_Q=\frac43C_M^2.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
