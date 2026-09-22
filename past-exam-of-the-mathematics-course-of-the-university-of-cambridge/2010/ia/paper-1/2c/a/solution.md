<h1 id="2c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [polar form of a complex number](../../../../../../polar-form-of-a-complex-number.md) and the [roots of unity](../../../../../../root-of-unity.md) give

$$
z_1=e^{2\pi i j/3},\quad j=0,1,2,
\qquad z_2=2e^{2\pi i k/9},\quad k=0,\ldots,8,
$$

since $512=2^9$. Using the [complex conjugate](../../../../../../complex-conjugate.md) to compute the squared [complex modulus](../../../../../../complex-modulus.md),

$$
|z_1-z_2|^2=|z_1|^2+|z_2|^2-2\operatorname{Re}(z_1\overline{z_2})
=5-4\cos\frac{2\pi(3j-k)}9.
$$

The residue $3j-k$ runs through every class modulo $9$, already with $j=0$. The [cosine](../../../../../../cosine.md) is even, so the nine angles give five distinct values, represented by $r=0,1,2,3,4$. They are distinct because [cosine](../../../../../../cosine.md) is strictly decreasing on $[0,\pi]$ and these representative angles lie in that interval. Hence

$$
\boxed{|z_1-z_2|\in
\left\{1,\sqrt{5-4\cos\frac{2\pi}9},
\sqrt{5-4\cos\frac{4\pi}9},\sqrt7,
\sqrt{5-4\cos\frac{8\pi}9}\right\}.}
$$

Every listed value is attained by choosing $z_1=1$ and $z_2=2e^{2\pi i r/9}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2C](../../2c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
