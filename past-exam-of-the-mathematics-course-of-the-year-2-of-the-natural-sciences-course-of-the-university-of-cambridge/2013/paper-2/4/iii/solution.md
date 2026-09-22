<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $\varepsilon\ne0$, use $z=e^{i\theta}$. The interval traverses $|z|=1$ once counterclockwise, $\cos\theta=(z+z^{-1})/2$, and $d\theta=dz/(iz)$. Thus

$$
I(\varepsilon)=\oint_{|z|=1}\frac{2\,dz}{i(\varepsilon z^2+2z+\varepsilon)}.
$$

Put $d=\sqrt{1-\varepsilon^2}>0$. The two simple poles are

$$
z_+=\frac{-1+d}{\varepsilon}=-\frac{\varepsilon}{1+d},\qquad z_-=-\frac{1+d}{\varepsilon}.
$$

Their moduli are $|\varepsilon|/(1+d)<1$ and $(1+d)/|\varepsilon|>1$, so exactly $z_+$ is enclosed, for either sign of $\varepsilon$. Its [residue](../../../../../residue.md) is

$$
\frac{2}{i(2\varepsilon z_++2)}=\frac1{id}.
$$

The [residue theorem](../../../../../residue-theorem.md) yields

$$
\boxed{I(\varepsilon)=\frac{2\pi}{\sqrt{1-\varepsilon^2}},\qquad -1<\varepsilon<1.}
$$

This also follows from the [reciprocal affine sine integral](../../../../../reciprocal-affine-sine-integral.md) after an angular shift. At $\varepsilon=0$, the original integral is directly $2\pi$, agreeing with the boxed formula. **The displayed two-pole formulas require $\varepsilon\ne0$**: at zero the contour integrand reduces to $1/(iz)$ with a single pole. Thus the source's claim of two simple poles has this removable special-case exception.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
