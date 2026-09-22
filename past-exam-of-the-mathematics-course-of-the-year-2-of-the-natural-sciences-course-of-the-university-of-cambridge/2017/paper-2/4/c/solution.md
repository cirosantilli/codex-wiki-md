<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First use $\sin\theta/(a-\sin\theta)=a/(a-\sin\theta)-1$. If $J=\int_{-\pi}^{\pi}(a-\sin\theta)^{-1}\,d\theta$, the required integral is $aJ-2\pi$.

Set $z=e^{i\theta}$. The [unit circle](../../../../../complex-unit-circle.md) is traversed counterclockwise once, $d\theta=dz/(iz)$, and $\sin\theta=(z-z^{-1})/(2i)$. Thus

$$
J=\frac1i\oint_{|z|=1}\frac{h(z)}z\,dz.
$$

The function $h(z)/z=-2i/(z^2-2iaz-1)$ is regular at zero. Its only enclosed [pole](../../../../../pole.md) is $z_-$ from part (b), and its [residue](../../../../../residue.md) is

$$
\operatorname{Res}_{z=z_-}\frac{h(z)}z=\frac1{z_-}\operatorname{Res}_{z=z_-}h=\frac1\Delta.
$$

By the [residue theorem](../../../../../residue-theorem.md), $J=(1/i)2\pi i/\Delta=2\pi/\Delta$. Therefore

$$
\boxed{\int_{-\pi}^{\pi}\frac{\sin\theta}{a-\sin\theta}\,d\theta=2\pi\left(\frac{a}{\sqrt{a^2-1}}-1\right).}
$$

As a sign and scale check, this is positive and behaves as $\pi/a^2$ for large $a$, in agreement with expanding the integrand and integrating its first nonzero, $\sin^2\theta/a^2$, term.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
