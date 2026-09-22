<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $i\ne j$, the [inertia tensor](../../../../../inertia-tensor.md) component is $I_{ij}=-\rho\int_Vx_ix_j\,dV$. Reflect either coordinate appearing once: the cylindrical domain and density are unchanged, while the integrand changes sign. Thus every off-diagonal component vanishes. Rotational symmetry also implies $I_{11}=I_{22}$.

Use [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) $x_1=r\cos\theta$, $x_2=r\sin\theta$, $x_3=z$, with volume element $r\,dr\,d\theta\,dz$. The axial [moment of inertia](../../../../../moment-of-inertia.md) is

$$
I_{33}=\rho\int_{-2}^{2}dz\int_0^{2\pi}d\theta\int_0^1r^3\,dr=2\pi\rho.
$$

The two contributions to a transverse component are

$$
\int_Vx_2^2\,dV=4\left(\int_0^1r^3dr\right)\left(\int_0^{2\pi}\sin^2\theta\,d\theta\right)=\pi,
\qquad\int_Vz^2\,dV=\pi\int_{-2}^{2}z^2dz=\frac{16\pi}{3}.
$$

Therefore

$$
\boxed{I=\pi\rho\,\operatorname{diag}\left(\frac{19}{3},\frac{19}{3},2\right)=M\operatorname{diag}\left(\frac{19}{12},\frac{19}{12},\frac12\right),\qquad M=4\pi\rho.}
$$

The axial value $MR^2/2$ and transverse value $M(3R^2+h^2)/12$ for $R=1$, $h=4$ give an independent check on both diagonal entries.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
