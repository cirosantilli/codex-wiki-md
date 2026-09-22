<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [unit normal](../../../../unit-normal.md) from part (c), and orient $\gamma_a$ by increasing $v$. Write $T=\gamma_a'/|\gamma_a'|$ for its [unit tangent vector](../../../../unit-tangent-vector.md). The signed [geodesic curvature](../../../../geodesic-curvature.md) convention used below is

$$
\kappa_g=\frac{dT}{ds}\cdot(N\times T)
=\frac{N\cdot(\gamma_a'\times\gamma_a'')}{|\gamma_a'|^3},
$$

where $s$ is [arc length](../../../../arc-length.md). The second equality follows by differentiating $T$: the term parallel to $\gamma_a'$ disappears in the [scalar triple product](../../../../scalar-triple-product.md). It makes the correction for a parameter which is not [arc-length parametrization](../../../../arc-length-parametrization.md) explicit.

Put $C=\cos a$, $S=\sin a$, $D=1+S^2$, and $G=3+2C$. The [speed](../../../../speed.md) is the constant $\sqrt G$. At $v=0$,

$$
\gamma_a'=(-S,1+C,1),\qquad \gamma_a''=(-1-C,-S,0),
$$

so

$$
\gamma_a'\times\gamma_a''=(S,-1-C,(1+C)^2+S^2)
=(S,-1-C,2+2C).
$$

Taking its [dot product](../../../../dot-product.md) with $N=(C,S,-S)/\sqrt D$ yields $-S(3+2C)/\sqrt D=-SG/\sqrt D$. Therefore

$$
\boxed{\kappa_g(\gamma_a)=-\frac{\sin a}{\sqrt{1+\sin^2a}\sqrt{3+2\cos a}},\qquad ds=\sqrt{3+2\cos a}\,dv.}
$$

The [screw motion](../../../../screw-motion.md) of part (b) makes this independent of $v$. Thus $\gamma_a$ is a [geodesic](../../../../geodesic.md) precisely when $a$ is an integer multiple of $\pi$. Reversing the direction of traversal or the [unit normal](../../../../unit-normal.md) changes the sign of signed [geodesic curvature](../../../../geodesic-curvature.md); its magnitude is the absolute value of the displayed expression. The signed convention is needed in part (e).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geometry of surfaces course of the University of Oxford](../../../split.md)
5. [Geometry of surfaces course of the University of Oxford](../../../../geometry-of-surfaces-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
