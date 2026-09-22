<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First interpret the [surface integral](../../../../surface-integral.md) through the given [parametric surface](../../../../parametric-surface.md), counting multiplicity. Set

$$
J(u)=\frac{\sin u}{\sqrt{1+\sin^2u}}.
$$

Its [derivative](../../../../derivative.md) is

$$
J'(u)=\frac{\cos u}{\sqrt{1+\sin^2u}}-\frac{\sin^2u\cos u}{(1+\sin^2u)^{3/2}}
=\frac{\cos u}{(1+\sin^2u)^{3/2}}.
$$

Using part (c), the [fundamental theorem of calculus](../../../../fundamental-theorem-of-calculus.md) gives

$$
\int_c^d\int_a^b\kappa(\mathbf r(u,v))\sqrt{EG-F^2}\,du\,dv
=(d-c)\bigl(J(b)-J(a)\bigr).
$$

On the other hand part (d), including its [arc length](../../../../arc-length.md) factor, gives

$$
\int_{\gamma_a([c,d])}\kappa_g\,ds
=-\int_c^d\frac{\sin a}{\sqrt{1+\sin^2a}}\,dv=-(d-c)J(a),
$$

and the corresponding expression for $b$ is $-(d-c)J(b)$. Subtraction proves

$$
\boxed{\int_c^d\int_a^b\kappa(\mathbf r(u,v))\sqrt{EG-F^2}\,du\,dv
=\int_{\gamma_a([c,d])}\kappa_g\,ds-\int_{\gamma_b([c,d])}\kappa_g\,ds.}
$$

If $0<b-a<2\pi$, the [parametric surface](../../../../parametric-surface.md) is [injective](../../../../injective-function.md) on the rectangle, so this is exactly the stated [surface integral](../../../../surface-integral.md) over its image. It also remains the ordinary image integral at $b-a=2\pi$, since the repeated seam has zero [surface area](../../../../surface-area.md).

**The assertion for arbitrary $a<b$ needs a multiplicity convention or the restriction $b-a\leq2\pi$.** This omission is present in the native PDF. For example, take $a=0$, $b=5\pi/2$, $c=0$, $d=1$. The image is the entire cylindrical band $0\leq z\leq1$, since $u$ already covers a full turn. Its ordinary [surface integral](../../../../surface-integral.md) of [Gaussian curvature](../../../../gaussian-curvature.md) is

$$
\int_0^1\int_0^{2\pi}\frac{\cos u}{(1+\sin^2u)^{3/2}}\,du\,dv=J(2\pi)-J(0)=0.
$$

But the difference of the two signed [geodesic curvature](../../../../geodesic-curvature.md) integrals is $J(5\pi/2)-J(0)=1/\sqrt2$. Thus ordinary integration over the image set makes the unrestricted assertion false. The boxed parameter integral is valid for all $a<b$ and $c<d$ and is the appropriate corrected statement. This distinction is the [multiplicity of a parametrized surface integral](../../../../multiplicity-of-a-parametrized-surface-integral.md).

## ↑ Ancestors (12)

1. [E](../e.md)
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
