<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

For the unheaded continuation, set $w=\log z$ in the food equation. The two square roots are $w=\pm i\pi/4$, so exponentiating gives

$$
\boxed{z=e^{i\pi/4},\ e^{-i\pi/4}=\frac{1\pm i}{\sqrt2}\quad\text{(food)}.}
$$

Both values have $|z-1|^2=2-\sqrt2<1$ and hence lie strictly inside the disk. Both also have the indicated principal logarithms. Allowing the multivalued [complex logarithm](../../../../../complex-logarithm.md) produces no additional points: the only permitted values of $w$ are still the two square roots already used.

For drink, the PDF squares only the denominator. Put $z=x+iy$. Its numerator is $(3x+iy)/2$ and its unsquared denominator is $(x+3iy)/2$, which is nonzero unless $z=0$. Multiplying the equation by this denominator squared and equating the [real part](../../../../../real-part.md) and [imaginary part](../../../../../imaginary-part.md) yields

$$
\frac32x=\frac34x^2-\frac{27}4y^2,\qquad\frac12y=\frac92xy,
$$

that is $x^2-9y^2=2x$ and $y(1-9x)=0$. If $y=0$, the real equation gives $x=0$ or $x=2$, and zero is excluded. If $y\ne0$, then $x=1/9$, but the real equation would require $9y^2=-17/81$, impossible for real $y$. Thus

$$
\boxed{z=2\quad\text{is the only drink point}.}
$$

It lies on the allowed disk boundary, and direct substitution gives $3/1^2=3$. The denominator-only square matters: squaring the entire quotient would define a different locus.

<a id="5c/image-food-points-inside-the-allowed-complex-disk-and-the-unique-drink-point-on-its-boundary"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-1-complex-locations.png)

**[Figure 1](#5c/image-food-points-inside-the-allowed-complex-disk-and-the-unique-drink-point-on-its-boundary). Food points inside the allowed complex disk and the unique drink point on its boundary**.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
