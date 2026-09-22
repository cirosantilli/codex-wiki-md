<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Write $R=a+b\cos u>0$. The tangent vectors are

$$
\sigma_u=(-b\sin u\cos v,-b\sin u\sin v,b\cos u),\qquad \sigma_v=(-R\sin v,R\cos v,0).
$$

Their squared lengths and inner product give the [first fundamental form](../../../../../first-fundamental-form.md)

$$
I=b^2\,du^2+R^2\,dv^2.
$$

The unit normal determined by this ordered parametrization is

$$
\nu=\frac{\sigma_u\times\sigma_v}{|\sigma_u\times\sigma_v|}=-(\cos u\cos v,\cos u\sin v,\sin u).
$$

Taking inner products of $\nu$ with $\sigma_{uu}$, $\sigma_{uv}$ and $\sigma_{vv}$ yields $e=b$, $f=0$, $g=R\cos u$. Consequently the [second fundamental form of a ring torus](../../../../../second-fundamental-form-of-a-ring-torus.md) is

$$
\boxed{II=b\,du^2+(a+b\cos u)\cos u\,dv^2.}
$$

This normal points into the tube. Choosing the outward unit normal reverses both coefficients and gives $-II$; the choice must therefore accompany an answer for the [second fundamental form](../../../../../second-fundamental-form-split.md).

The [Gaussian curvature](../../../../../gaussian-curvature.md) is unchanged by that reversal:

$$
\boxed{K=\frac{eg-f^2}{EG-F^2}=\frac{\cos u}{b(a+b\cos u)}.}
$$

Since the denominator is positive, $K>0$ on the outside of the [torus](../../../../../torus.md), where $\cos u>0$, and $K<0$ on its inner side, where $\cos u<0$. It vanishes on the two circles $u=\pi/2,3\pi/2$. This is the [Gaussian curvature of a ring torus](../../../../../gaussian-curvature-of-a-ring-torus.md).

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
