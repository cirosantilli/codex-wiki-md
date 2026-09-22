<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For radial motion, take an [affine parameter](../../../../../../affine-parameter.md) $\lambda$ and use dots for $d/d\lambda$. The [radial null geodesics of the Vaidya metric](../../../../../../radial-null-geodesics-of-the-vaidya-metric.md) satisfy the two radial [geodesic equations](../../../../../../geodesic-equation.md)

$$
\ddot v+\frac Mr^2\dot v^2=0,
\qquad
\ddot r+\left(\frac{fM}{r^2}+\frac{M'}r\right)\dot v^2-\frac{2M}{r^2}\dot v\dot r=0.
$$

The radial squared norm is $-f\dot v^2+2\dot v\dot r$. If $v$ is constant it vanishes, and the [geodesic equation](../../../../../../geodesic-equation.md) reduces to $\ddot r=0$. Thus **constant-$v$ radial curves are null geodesics**, with $r=a\lambda+b$ an affine parametrization. Future ingoing motion has $a<0$.

For the other family let $dr/dv=f/2$. Its tangent $k=\partial_v+(f/2)\partial_r$ is a [null vector](../../../../../../null-vector.md). Using the [Christoffel symbols of the Vaidya metric](../../../../../../christoffel-symbols-of-the-vaidya-metric.md), direct differentiation gives

$$
\nabla_kk=\frac{f_r}{2}k=\frac Mr^2k.
$$

Hence **these are also null geodesics, but $v$ is generally not affine**. For completeness, put $p=dv/d\lambda$ and choose

$$
\frac{d\log p}{dv}=-\frac{M(v)}{r(v)^2},
\qquad \frac{d\lambda}{dv}=C\exp\left(\int^v\frac{M(u)}{r(u)^2}\,du\right),\quad C\ne0.
$$

This makes $\ddot v=-(M/r^2)\dot v^2$. Differentiating $\dot r=(f/2)\dot v$ then gives $\ddot r=(f_v/2)\dot v^2=-M'\dot v^2/r$; substitution verifies the radial $r$ equation as well. Thus the [null condition](../../../../../../null-condition.md) and both radial [geodesic equations](../../../../../../geodesic-equation.md) hold, not just the null condition alone.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
