<h1 id="10/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take [spherical polar coordinates](../../../../../spherical-coordinate-system.md) with polar [angle](../../../../../angle.md) $\theta$ measured from positive $z$ and [azimuthal angle](../../../../../azimuthal-angle-in-cylindrical-coordinates.md) $\phi$:

$$
x=r\sin\theta\cos\phi,\qquad y=r\sin\theta\sin\phi,\qquad z=r\cos\theta.
$$

The derivative [matrix](../../../../../matrix.md) is

$$
\frac{\partial(x,y,z)}{\partial(r,\theta,\phi)}
=\begin{pmatrix}
\sin\theta\cos\phi&r\cos\theta\cos\phi&-r\sin\theta\sin\phi\\
\sin\theta\sin\phi&r\cos\theta\sin\phi&r\sin\theta\cos\phi\\
\cos\theta&-r\sin\theta&0
\end{pmatrix}.
$$

Expanding its [determinant](../../../../../determinant.md) gives $r^2\sin\theta$. Thus

$$
\boxed{dV=r^2\sin\theta\,dr\,d\theta\,d\phi,\qquad
\det\frac{\partial(r,\theta,\phi)}{\partial(x,y,z)}=\frac1{r^2\sin\theta}.}
$$

The inverse formula holds where $r>0$ and $0<\theta<\pi$; it excludes the origin and polar axis. These formulas use the general [chain rule](../../../../../chain-rule.md) and determinant construction in [solution](../i/solution.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [10](../../../10.md)
4. [2019 resit](../../../../2019-resit-split.md)
5. [Past exam of the mathematical methods II course of the University of Oxford](../../../../split.md)
6. [Mathematical methods II course of the University of Oxford](../../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
