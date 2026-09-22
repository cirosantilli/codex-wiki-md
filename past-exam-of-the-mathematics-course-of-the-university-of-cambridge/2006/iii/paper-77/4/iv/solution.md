<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $Q_0>0$ denote the small excess PV in the spherical region, with $Q_0\ll|f|$ for quasi-geostrophic consistency. Let its stretched radius be $R$ and set $r=(X^2+Y^2+Z^2)^{1/2}$. Spherical symmetry of the source and uniqueness of the decaying inversion imply a radial [streamfunction](../../../../../../stream-function.md). Its equations are

$$
\frac1{r^2}\frac d{dr}(r^2\psi_r)=\begin{cases}Q_0,&r<R,\\0,&r>R.\end{cases}
$$

Regularity at the origin removes the interior $1/r$ term. Decay removes the exterior constant. Integrating gives $\psi_{
m in}=Q_0r^2/6+C_0$ and $\psi_{
m out}=C_1/r$. Since the source has no surface delta function, $\psi$ and $\psi_r$ match at $R$. Their matching fixes $C_1=-Q_0R^3/3$ and $C_0=-Q_0R^2/2$. Therefore the [spherical potential-vorticity anomaly](../../../../../../spherical-potential-vorticity-anomaly.md) has

$$
\boxed{\psi(r)=\begin{cases}
\dfrac{Q_0}{6}(r^2-3R^2),&r\leq R,\\[4pt]
-\dfrac{Q_0R^3}{3r},&r\geq R.
\end{cases}}
$$

Its induced horizontal flow is

$$
(u_g,v_g)=\begin{cases}
(Q_0/3)(-y,x),&r<R,\\
[Q_0R^3/(3r^3)](-y,x),&r>R.
\end{cases}
$$

This flow is azimuthal about the vertical axis, so it is tangent to the PV level surfaces and advects no part of this axisymmetric distribution across its spherical boundary. The example is therefore steady under the quasi-geostrophic PV evolution. In physical coordinates the stretched sphere is the ellipsoid $x^2+y^2+(N^2/f^2)z^2=R^2$, with vertical semiaxis $R|f|/N$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
