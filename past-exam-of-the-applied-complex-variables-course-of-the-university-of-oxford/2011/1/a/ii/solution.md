<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The two approaches to the slit base are distinct [boundary](../../../../../boundary-of-a-set.md) points, each with interior [angle](../../../../../angle.md) $\pi/2$, whereas the slit tip has interior [angle](../../../../../angle.md) $2\pi$. Their exponents in the [Schwarz-Christoffel formula](../../../../../schwarz-christoffel-mapping.md) are therefore $-1/2$, $1$ and $-1/2$. Write $a=x_2\in(-1,1)$ and take

$$
S(z)=\sqrt{z^2-1}
$$

on the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md), with the branch normalized by $S(z)\sim z$ at [infinity](../../../../../infinity.md). The [derivative](../../../../../derivative.md) has the form

$$
f'(z)=c\frac{z-a}{S(z)}.
$$

On $-1<x<1$, the upper [boundary value](../../../../../boundary-value.md) is $S_+(x)=i\sqrt{1-x^2}$. Both endpoints of this interval map to the slit base, so

$$
0=f(1)-f(-1)=c\int_{-1}^1\frac{x-a}{i\sqrt{1-x^2}}\,dx=i\pi ca.
$$

The odd term integrates to zero, and $c\ne0$; hence $\boxed{x_2=0}$. Now $S'(z)=z/S(z)$, so $f=cS+b$. The endpoint values force $b=0$, and the tip value, using $S(0)=i$ as a [boundary](../../../../../boundary-of-a-set.md) limit, forces $c=1$. Thus

$$
\boxed{f(z)=\sqrt{z^2-1},\qquad f(z)\sim z\text{ at infinity}.}
$$

The branch is important: on $x>1$ its [boundary value](../../../../../boundary-value.md) is positive real, on $x<-1$ negative real, and on $(-1,1)$ positive imaginary. The intervals $(-1,0)$ and $(0,1)$ traverse the two sides of the slit, meeting at its tip.

The map is injective in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md): equal images imply $z_1^2=z_2^2$, and the alternative $z_1=-z_2$ cannot put both points in that half-plane. Its [derivative](../../../../../derivative.md) has no interior zero. The image has positive [imaginary part](../../../../../imaginary-part.md), by [continuity](../../../../../continuous-function.md) of the branch and the fact that an interior real image would require $z^2-1$ to be nonnegative real, which is impossible for $\operatorname{Im}z>0$. Conversely, a point $\zeta$ in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) outside the slit gives a unique upper-half-plane root of $z^2=\zeta^2+1$. A point $\zeta=iy$ with $0<y\leq1$ gives only real roots or zero and is excluded. These observations verify that the image is exactly the required slit domain, rather than just matching its [boundary](../../../../../boundary-of-a-set.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the applied complex variables course of the University of Oxford](../../../../split.md)
6. [Applied complex variables course of the University of Oxford](../../../../../applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
