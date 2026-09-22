<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With $s=r\sin\theta$ and $z=r\cos\theta$, radial [differential rotation](../../../../../../differential-rotation.md) gives $\partial_z\omega=\cos\theta\,\omega'(r)$. Thus the source is $B_0r\omega'(r)\sin\theta\cos\theta$. Put $B=f(r)g(\theta)$ with $g=\sin\theta\cos\theta$. The toroidal diffusion operator is

$$
\left(\nabla^2-\frac1{s^2}\right)(fg)=\left(f''+\frac2rf'\right)g+\frac f{r^2}\left[\frac1{\sin\theta}\frac d{d\theta}\left(\sin\theta\frac{dg}{d\theta}\right)-\frac g{\sin^2\theta}\right].
$$

Direct differentiation of $g$ makes the bracket $-6g$. Therefore the steady radial equation is

$$
\eta\left(f''+\frac2rf'-\frac6{r^2}f\right)=-B_0r\omega'(r).
$$

Define $I(r)=\int_0^r x^4\omega(x)\,dx$ and $h=I/r^3$. Since $I'=r^4\omega$,

$$
h'=r\omega-\frac{3I}{r^4},\qquad h''=r\omega'-2\omega+\frac{12I}{r^5},
$$

so $h''+2h'/r-6h/r^2=r\omega'$. Taking $f=-B_0h/\eta$ proves the [steady toroidal induction by spherical differential rotation](../../../../../../steady-toroidal-induction-by-spherical-differential-rotation.md):

$$
\boxed{B(r,\theta)=-\frac{B_0}{\eta}\frac{\sin\theta\cos\theta}{r^3}\int_0^rx^4\omega(x)\,dx.}
$$

Near zero, $I(r)=\omega(0)r^5/5+O(r^6)$, hence $B=O(r^2)\sin\theta\cos\theta$ and is regular. Its leading [vector field](../../../../../../vector-field.md) is proportional to $z(-y,x,0)$, so the apparent azimuthal-basis singularity on the axis is harmless. The rapid decay of $\omega$ makes $I_\infty=\int_0^\infty x^4\omega(x)\,dx$ finite, giving $B\sim-(B_0I_\infty/\eta)r^{-3}\sin\theta\cos\theta$ at large radius. The homogeneous radial solutions are $r^2$ and $r^{-3}$; regularity at zero excludes the latter, and decay at infinity excludes the former. Thus these boundary requirements also single out the displayed solution in this angular sector.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
