<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a positively oriented simple closed [contour](../../../../../complex-integration-contour.md), the [residue theorem](../../../../../residue-theorem.md) states that the integral of a function holomorphic on and inside the [contour](../../../../../complex-integration-contour.md) except at finitely many isolated interior singularities is $2\pi i$ times the sum of its [residues](../../../../../residue.md). There must be no singularity on the [contour](../../../../../complex-integration-contour.md).

Factor the denominator as $(z^2+z+1)(z^2-z+1)$. For $R>1$, the upper semicircle encloses the two [simple poles](../../../../../simple-pole.md)

$$
a=\frac12+\frac{i\sqrt3}{2},\qquad b=-\frac12+\frac{i\sqrt3}{2}.
$$

The other two [poles](../../../../../pole.md) are in the lower half-plane. Since $D'(z)=4z^3+2z=2z(2z^2+1)$,

$$
\operatorname{Res}_{a}g=\frac{e^{ia}}{2i\sqrt3\,a},\qquad
\operatorname{Res}_{b}g=-\frac{e^{ib}}{2i\sqrt3\,b}.
$$

Writing $h=\sqrt3/2$ and using $1/a=1/2-ih$, $1/b=-1/2-ih$, their numerator difference simplifies to

$$
\frac{e^{ia}}a-\frac{e^{ib}}b
=e^{-h}\left[\left(\frac12-ih\right)e^{i/2}+\left(\frac12+ih\right)e^{-i/2}\right]
=e^{-h}\left[\cos\frac12+\sqrt3\sin\frac12\right].
$$

Thus for every $R>1$ the closed-contour integral is

$$
\oint_{L_R\cup C_R}g(z)\,dz
=\frac\pi{\sqrt3}e^{-\sqrt3/2}\left[\cos\frac12+\sqrt3\sin\frac12\right].
$$

To remove the arc, on $C_R$ we have $|e^{iz}|=e^{-\operatorname{Im}z}\leq1$ and $|z^4+z^2+1|\geq R^4-R^2-1$. For sufficiently large $R$, the [complex line integral estimate](../../../../../complex-line-integral-estimate.md) gives

$$
\left|\int_{C_R}g(z)\,dz\right|
\leq\frac{\pi R}{R^4-R^2-1}\longrightarrow0.
$$

The real-line integral is absolutely convergent. Its imaginary part is zero by oddness of $\sin x/(x^4+x^2+1)$. Therefore

$$
\boxed{\int_{-\infty}^{\infty}\frac{\cos x}{x^4+x^2+1}\,dx
=\frac\pi{\sqrt3}e^{-\sqrt3/2}\left[\cos\frac12+\sqrt3\sin\frac12\right]}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
