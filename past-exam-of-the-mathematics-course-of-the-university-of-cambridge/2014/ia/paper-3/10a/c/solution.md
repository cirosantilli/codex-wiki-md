<h1 id="10a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Direct use of [partial derivatives](../../../../../../partial-derivative.md) gives

$$
\boxed{\nabla\times\mathbf F=(x^2+2xy,-2xy-y^2,2).}
$$

With the upward [oriented surface element](../../../../../../oriented-surface-element.md) found in part (b), the [curl](../../../../../../curl.md) flux integrand over the [annulus](../../../../../../annulus-mathematics.md) $A$ becomes

$$
2+\frac{-x^3-2x^2y+2xy^2+y^3}{\sqrt{1+x^2+y^2}}.
$$

Every term in the numerator is odd in $x$ or $y$, so its integral over the symmetric [annulus](../../../../../../annulus-mathematics.md) is zero. Thus the [surface integral](../../../../../../surface-integral.md) is

$$
\int_S(\nabla\times\mathbf F)\cdot d\mathbf S
=2\operatorname{Area}(A)=2\pi(2^2-1^2)=6\pi.
$$

Each boundary circle has constant $z$, hence $dz=0$. Its [line integral](../../../../../../line-integral.md) is therefore $\int(-y\,dx+x\,dy)$, with no contribution from the third field component. An anticlockwise radius-$r$ circle gives $2\pi r^2$. The outward boundary orientation is anticlockwise at $r=2$ and clockwise at $r=1$, so

$$
\oint_{\partial S}\mathbf F\cdot d\mathbf x=8\pi-2\pi=\boxed{6\pi}.
$$

The two computed values agree, verifying [Stokes theorem](../../../../../../stokes-theorem.md) with both boundary components. A downward choice would give $-6\pi$ on both sides.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10A](../../10a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
