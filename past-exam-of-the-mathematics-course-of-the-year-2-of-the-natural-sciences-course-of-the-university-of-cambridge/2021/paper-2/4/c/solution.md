<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $z=e^{i\theta}$. Then $d\theta=dz/(iz)$ and $\tan\theta=(z^2-1)/[i(z^2+1)]$, so the requested integral is

$$
I=\frac1i\oint_{|z|=1}f(z)\,dz,\qquad f(z)=\frac{(1+z^2)^2}{z[a^2(1+z^2)^2-(1-z^2)^2]}.
$$

The denominator factors as

$$
[(a-1)+(a+1)z^2][(a+1)+(a-1)z^2].
$$

For $0<a<1$, its two inner roots are $z=\pm r$, $r=\sqrt{(1-a)/(1+a)}<1$, and the other two roots have modulus $1/r>1$. There is also a [simple pole](../../../../../simple-pole.md) at zero. Their [residues](../../../../../residue.md) are

$$
\operatorname{Res}_{0}f=\frac1{a^2-1},\qquad\operatorname{Res}_{\pm r}f=\frac1{2a(1-a^2)}.
$$

The latter values follow by differentiating the quadratic product, or from the supplied hint. The sum of the enclosed [residues](../../../../../residue.md) is

$$
-\frac1{1-a^2}+\frac1{a(1-a^2)}=\frac1{a(1+a)}.
$$

The [residue theorem](../../../../../residue-theorem.md) therefore gives

$$
\boxed{I=\frac{2\pi}{a(1+a)},\qquad\mathcal C=2\pi.}
$$

At the angles where the tangent is undefined, the original reciprocal has a removable zero limit. Its continuous extension gives the same integral; the transformed rational integrand has no [pole](../../../../../pole.md) on the [unit circle](../../../../../complex-unit-circle.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
