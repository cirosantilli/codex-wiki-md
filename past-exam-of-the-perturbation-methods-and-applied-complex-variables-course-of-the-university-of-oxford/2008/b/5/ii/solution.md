<h1 id="b/5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The finite corners have interior angle $3\pi/2$, hence exterior-angle parameters $-1/2$. The channel end at $Z=0$ is logarithmic. Their [Schwarz-Christoffel mapping](../../../../../schwarz-christoffel-mapping.md) is consequently

$$
f'(Z)=C\frac{\sqrt{Z^2-1}}{Z}.
$$

Choose $R(Z)=\sqrt{Z^2-1}$ analytic in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) with $R(Z)\sim Z$ at upper infinity. In particular $R(iy)=i\sqrt{1+y^2}$ for $y>0$. A direct differentiation gives

$$
\frac d{dZ}\left(R+\tan^{-1}\frac1R\right)
=\frac ZR-\frac1{ZR}=\frac RZ.
$$

Hence $f=A+C H$ with $H=R+\tan^{-1}(1/R)$.

The [inverse trigonometric functions](../../../../../inverse-trigonometric-functions.md) here is the branch obtained by [analytic continuation](../../../../../analytic-continuation.md) from $Z>1$ through the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md), not an independent [Cauchy principal value](../../../../../cauchy-principal-value.md) evaluation at each point. Its endpoint values give $H(1)=\pi/2$, $H(-1)=-\pi/2$. Imposing $f(1)=1$ and $f(-1)=-1$ therefore gives $A=0$, $C=2/\pi$:

$$
\boxed{z=\frac2\pi\left(\sqrt{Z^2-1}
+\tan^{-1}(Z^2-1)^{-1/2}\right).}
$$

Along the positive imaginary axis, $H$ is purely imaginary and tends to $-i\infty$ as $Z\to0$; at upper infinity $H\sim Z$. The real intervals $(0,1)$ and $(-1,0)$ trace the channel walls $x=1$ and $x=-1$ downward, while the outer intervals trace the horizontal boundary. This verifies the stated end assignments as well as the constants. The map is the [Schwarz-Christoffel map of a half-plane joined to a strip](../../../../../schwarz-christoffel-map-of-a-half-plane-joined-to-a-strip.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
