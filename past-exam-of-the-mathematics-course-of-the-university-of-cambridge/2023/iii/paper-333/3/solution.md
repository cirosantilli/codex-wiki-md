<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The interior equation materially conserves [three-dimensional quasi-geostrophic potential vorticity](../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md). At each rigid horizontal boundary, $\psi_z$ is proportional to the boundary buoyancy anomaly, so the other two equations express material conservation of that buoyancy.

A background streamfunction $\overline\psi=-\Lambda zy$ gives $\overline{\mathbf u}_g=(\Lambda z,0,0)$. Its interior PV is uniform. Writing $\psi=\overline\psi+\psi'$ and retaining first-order terms gives

$$
\boxed{
(\partial_t+\Lambda z\partial_x)
(\psi'_{xx}+\psi'_{yy}+f^2N^{-2}\psi'_{zz})=0}
$$

in the interior. Since $\overline\psi_z=-\Lambda y$, perturbation advection of the boundary buoyancy gives

$$
\boxed{
(\partial_t+\Lambda z\partial_x)\psi'_z
-\Lambda\psi'_x=0}
$$

at $z=0,H$. At the lower boundary this is replaced by

$$
(\partial_t\psi'_z-\Lambda\psi'_x)_{z=0}
=-\alpha\psi'_z(0).
$$

For a Fourier component $\widehat\psi(z,t)e^{ikx}$ with zero interior PV,

$$
\widehat\psi_{zz}-\frac{N^2k^2}{f^2}\widehat\psi=0.
$$

Solving this boundary-value problem in terms of

$$
q_0=\widehat\psi_z(0,t),
\qquad
q_H=\widehat\psi_z(H,t)
$$

gives

$$
\boxed{\widehat\psi(0)=-Aq_0+Bq_H,
\qquad
\widehat\psi(H)=-Bq_0+Aq_H},
$$

where, with $\mu=NHk/f$,

$$
\boxed{A=\frac f{Nk}\coth\mu,
\qquad
B=\frac f{Nk}\operatorname{csch}\mu}.
$$

The boundary equations consequently reduce to

$$
\boxed{
\dot q_0+(\alpha+ik\Lambda A)q_0
-ik\Lambda Bq_H=0},
$$



$$
\boxed{
\dot q_H+ik\Lambda Bq_0
+ik\Lambda(H-A)q_H=0}.
$$

For $q_0,q_H\propto e^{-ikct}$, define

$$
\widetilde c=\frac c{\Lambda H},
\qquad
\epsilon=\frac\alpha{k\Lambda H}.
$$

The determinant gives the [Damped Eady-wave dispersion relation](../../../../../damped-eady-wave-dispersion-relation.md)

$$
\boxed{
\widetilde c_\pm=\frac12(1-i\epsilon)
\pm\sqrt{
\frac1{\mu^2}-\frac{\coth\mu}{\mu}+\frac14
+i\epsilon\left(\frac12-\frac{\coth\mu}{\mu}\right)
-\frac{\epsilon^2}{4}}}.
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
