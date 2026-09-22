<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $d=\sqrt{a^2-b^2}>0$. The two roots are

$$
z_{\rm in}=-i\frac{a-d}{b},\qquad z_{\rm out}=-i\frac{a+d}{b}.
$$

Since $(a-d)(a+d)=b^2$, their moduli are $b/(a+d)<1$ and $(a+d)/b>1$. Thus exactly one root is inside the unit circle, and neither lies on it.

For the real integral use $z=e^{i\theta}$, so $\sin\theta=(z-z^{-1})/(2i)$ and $d\theta=dz/(iz)$. The [change of variables](../../../../../change-of-variables-formula.md) gives

$$
\int_0^{2\pi}\frac{d\theta}{a+b\sin\theta}=\oint_{|z|=1}\frac{2\,dz}{bz^2+2iaz-b}.
$$

The contour is counterclockwise. At its single interior [simple pole](../../../../../simple-pole.md), the [residue](../../../../../residue.md) is

$$
\frac{2}{2bz_{\rm in}+2ia}=\frac1{id}.
$$

By the [residue theorem](../../../../../residue-theorem.md), the [reciprocal affine sine integral](../../../../../reciprocal-affine-sine-integral.md) is therefore

$$
\boxed{\int_0^{2\pi}\frac{d\theta}{a+b\sin\theta}=2\pi i\frac1{id}=\frac{2\pi}{\sqrt{a^2-b^2}}.}
$$

The condition $a>b>0$ also makes the real denominator strictly positive, consistent with the positive answer and the absence of contour poles on the unit circle.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
