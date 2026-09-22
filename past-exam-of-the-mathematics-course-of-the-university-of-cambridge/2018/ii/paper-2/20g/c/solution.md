<h1 id="20g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $L=\mathbb Q(\omega)$ and $F=\mathbb Q(\omega+\omega^{-1})$. The [maximal real subfield of the fifth cyclotomic field](../../../../../../maximal-real-subfield-of-the-fifth-cyclotomic-field.md) is $F=\mathbb Q(\sqrt5)$. The [roots of unity in a rational cyclotomic field](../../../../../../roots-of-unity-in-a-rational-cyclotomic-field.md) show that the roots of unity in $L$ are exactly $\{\mathord\pm\omega^a\}$.

Let $u\in\mathcal O_L^\times$. For every embedding $\sigma:L\to\mathbb C$,

$$
\left|\sigma\left(\frac{u}{\bar u}\right)\right|=1.
$$

Thus the [kernel of the logarithmic unit embedding](../../../../../../kernel-of-the-logarithmic-unit-embedding.md) implies that $u/\bar u$ is a root of unity. Since conjugation acts trivially modulo the prime element $1-\omega$, we have $u/\bar u\equiv1\pmod{1-\omega}$. Among the tenth roots of unity this excludes the elements $-\omega^a$, so $u/\bar u\in\langle\omega\rangle$. Squaring is a bijection on this group of order five, so choose a root of unity $\eta$ with $\eta/\bar\eta=u/\bar u$. Then $v=u/\eta$ is fixed by conjugation and is therefore a unit of $F$.

The [units of the quadratic field Q square root of five](../../../../../../units-of-the-quadratic-field-q-square-root-of-five.md) are $\mathord\pm\phi^b$, where $\phi=(1+\sqrt5)/2$. Absorbing the sign and $\eta$ into $\mathord\pm\omega^a$ proves

$$
\boxed{\mathcal O_L^\times
=\left\{\mathord\pm\omega^a
\left(\frac{1+\sqrt5}{2}\right)^b:a,b\in\mathbb Z\right\}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20G](../../20g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
