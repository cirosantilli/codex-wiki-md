<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set

$$
D(r)=b+(\sqrt b+\sqrt r)^2
=r+2\sqrt{br}+2b,
\qquad
\Psi(r)=-\Phi(r)=\frac{GM}{D(r)}.
$$

The spherical [Poisson equation](../../../../../../poisson-equation.md) gives

$$
\rho(r)=\frac1{4\pi G r^2}
\frac d{dr}\left(r^2\frac{d\Phi}{dr}\right)
=\frac{M[6b^{3/2}\sqrt r+10br+3\sqrt b\,r^{3/2}]}
{8\pi r^2D^3}.
$$

The numerator identity

$$
6b^{3/2}\sqrt r+10br+3\sqrt b\,r^{3/2}
=3\sqrt{br}\,D+4br
$$

splits this into two [scale-free density-potential components](../../../../../../scale-free-density-potential-component.md):

$$
\boxed{
\rho(r)=
\frac{3\sqrt b}{8\pi G^2M}r^{-3/2}\Psi^2
+\frac{b}{2\pi G^3M^2}r^{-1}\Psi^3}.
$$

Thus

$$
(\gamma_1,p_1,A_1)
=\left(\frac32,2,\frac{3\sqrt b}{8\pi G^2M}\right),
$$



$$
(\gamma_2,p_2,A_2)
=\left(1,3,\frac{b}{2\pi G^3M^2}\right).
$$

At small radius, $D\sim2b$ and the first term dominates:

$$
\rho(r)\sim\frac{3M}{32\pi b^{3/2}}r^{-3/2}.
$$

The cusp has finite enclosed mass because $r^2\rho\sim r^{1/2}$. Moreover,

$$
v_c^2=r\frac{d\Phi}{dr}
=\frac{GMr[1+\sqrt{b/r}]}{D^2}
\sim\frac{GM}{4b^{3/2}}\sqrt r,
$$

so the [circular speed](../../../../../../circular-speed.md) tends to zero as $r^{1/4}$. At large radius, $D\sim r$ and

$$
\rho(r)\sim\frac{3M\sqrt b}{8\pi}r^{-7/2}.
$$

Since $r^2\rho\sim r^{-3/2}$ is integrable at infinity and $\Phi\sim-GM/r$, the total mass is finite and equals $M$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
