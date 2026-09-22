<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On a [sphere](../../../../../../../sphere.md) of radius $r$, the radial [gravitational field](../../../../../../../gravitational-field.md) has constant magnitude. Thus [Gauss's law for gravity](../../../../../../../gauss-s-law-for-gravity.md) becomes

$$
4\pi r^2\varphi'(r)=-4\pi GM(r),\qquad
\varphi'(r)=-\frac{GM(r)}{r^2},
$$

where $M(r)$ is the enclosed [mass](../../../../../../../mass.md). In the hollow core $M(r)=0$. In the material shell, put $u=r/r_0$ and use the [spherical coordinates](../../../../../../../spherical-coordinate-system.md) volume element:

$$
\begin{aligned}
M(r)&=4\pi\rho_0r_0\int_{r_0}^r s e^{-s/r_0}\,ds\\
&=4\pi\rho_0r_0^3\int_1^u v e^{-v}\,dv
=4\pi\rho_0r_0^3\left[\frac2e-(u+1)e^{-u}\right],\qquad 1\leq u\leq2.
\end{aligned}
$$

Outside the shell the enclosed [mass](../../../../../../../mass.md) is the total

$$
M_*=4\pi\rho_0r_0^3\left(\frac2e-\frac3{e^2}\right).
$$

Consequently,

$$
\boxed{\varphi'(r)=
\begin{cases}
0,&0\leq r<r_0,\\
-\dfrac{4\pi G\rho_0r_0^3}{r^2}\left[\dfrac2e-\left(1+\dfrac r{r_0}\right)e^{-r/r_0}\right],&r_0\leq r\leq2r_0,\\
-\dfrac{4\pi G\rho_0r_0^3}{r^2}\left(\dfrac2e-\dfrac3{e^2}\right),&r>2r_0.
\end{cases}}
$$

At $r=0$ the displayed value refers to the radial [derivative](../../../../../../../derivative.md) of the constant core value. The expressions match at both shell boundaries. There is no surface sheet of [mass](../../../../../../../mass.md), so a jump in the volume [mass density](../../../../../../../density.md) does not produce a jump in the [gravitational field](../../../../../../../gravitational-field.md). The core has zero [gravitational field](../../../../../../../gravitational-field.md), and the exterior [gravitational field](../../../../../../../gravitational-field.md) equals that of a central [point mass](../../../../../../../point-mass.md) $M_*$, as in the [shell theorem](../../../../../../../spherical-shell-theorem.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
