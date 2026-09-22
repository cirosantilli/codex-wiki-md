<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

[Independence](../../../../../independent-random-variables.md) gives the joint [probability density function](../../../../../probability-density-function.md) $f_{X,Y}(x,y)=4e^{-(x^2+y^2)}/\pi$ on $x,y>0$. The inverse transformation is

$$
x=\sqrt{\frac{u}{1+v^2}},\qquad y=v\sqrt{\frac{u}{1+v^2}},\qquad u,v>0.
$$

Its [Jacobian matrix](../../../../../jacobian-matrix.md) has absolute determinant $1/[2(1+v^2)]$. One way to see the determinant is to use polar coordinates: $u=r^2$, $v=\tan\theta$, with $0<\theta<\pi/2$. Then $dx\,dy=r\,dr\,d\theta=du\,dv/[2(1+v^2)]$. The [change-of-variables formula for probability densities](../../../../../change-of-variables-formula-for-a-probability-density.md) gives

$$
\boxed{f_{U,V}(u,v)=\frac2\pi\frac{e^{-u}}{1+v^2},\qquad u,v>0,}
$$

and zero outside that support. Integrating over the complementary variable gives

$$
\boxed{f_U(u)=e^{-u}\ \ (u>0),\qquad f_V(v)=\frac2{\pi(1+v^2)}\ \ (v>0).}
$$

These are respectively a unit-rate [exponential distribution](../../../../../exponential-distribution.md) and a unit-scale [half-Cauchy distribution](../../../../../half-cauchy-distribution.md). Their product equals the [joint probability density function](../../../../../joint-probability-density.md), so **$U$ and $V$ are independent**. This [radial-ratio independence of two half-normal variables](../../../../../radial-ratio-independence-of-two-half-normal-variables.md) results from the radial symmetry of the positive-quadrant [joint probability density function](../../../../../joint-probability-density.md).

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
