<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $d=\sqrt{a^2-b^2-c^2}>0$ and $h=b-ic$. The denominator of the complex [rational function](../../../../rational-function.md) becomes

$$
P(z)=\frac h2z^2+az+\frac{b+ic}{2}.
$$

The [quadratic formula](../../../../quadratic-formula.md) gives its two zeros, hence the two [poles](../../../../pole.md):

$$
\boxed{z_{\rm in}=\frac{-a+d}{b-ic},\qquad z_{\rm out}=\frac{-a-d}{b-ic}.}
$$

Their product is $(b+ic)/(b-ic)$, so $|z_{\rm in}z_{\rm out}|=1$. To locate them one also needs to exclude the possibility of both lying on the [unit circle](../../../../complex-unit-circle.md). Here their moduli are explicit:

$$
|z_{\rm in}|=\frac{a-d}{\sqrt{b^2+c^2}}=\sqrt{\frac{a-d}{a+d}}<1,\qquad
|z_{\rm out}|=\sqrt{\frac{a+d}{a-d}}>1.
$$

Both are [simple poles](../../../../simple-pole.md): $P'(z)=hz+a$ takes the nonzero values $d$ and $-d$ at them. In particular their [residues](../../../../residue.md) are $1/d$ and $-1/d$.

For the real [integral](../../../../integral-split.md), use the [change of variables](../../../../change-of-variables-formula.md) $z=e^{i\theta}$. As $\theta$ runs from $-\pi$ to $\pi$, this traverses the [unit circle](../../../../complex-unit-circle.md) once counterclockwise, and

$$
d\theta=\frac{dz}{iz},\quad\cos\theta=\frac{z+z^{-1}}2,\quad\sin\theta=\frac{z-z^{-1}}{2i}.
$$

Thus $I=(1/i)\oint_{|z|=1}f(z)dz$. Only $z_{\rm in}$ is enclosed. The [residue theorem](../../../../residue-theorem.md), or [Cauchy integral formula](../../../../cauchy-integral-formula.md) after subtracting its simple-pole part, gives

$$
\boxed{I=\frac1i\frac{2\pi i}{d}=\frac{2\pi}{\sqrt{a^2-b^2-c^2}}.}
$$

The real denominator is positive because $a>\sqrt{b^2+c^2}$. As an independent check, write $b\cos\theta+c\sin\theta=\sqrt{b^2+c^2}\cos(\theta-\phi)$; a period shift reduces the answer to the existing [reciprocal affine sine integral](../../../../reciprocal-affine-sine-integral.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
