<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the unitary [discrete Fourier transform](../../../../../../discrete-fourier-transform.md), with $e(x)=\exp(2\pi ix)$:

$$
\widehat f(a)=q^{-1/2}\sum_{n\bmod q}f(n)e(-an/q).
$$

For a unit $a$, substitute $m=an$ in the sum. The multiplicativity of the [Dirichlet character](../../../../../../dirichlet-character.md) gives $\chi(a^{-1}m)=\overline{\chi(a)}\chi(m)$, hence

$$
\boxed{\widehat\chi(a)=\overline{\chi(a)}\widehat\chi(1).}
$$

The [complex conjugation](../../../../../../complex-conjugation.md) is present in the original PDF and lost in the converted TeX. It matters for nonreal characters.

Now let $q=p^k$ and let $\chi$ be primitive. Since it does not descend to $p^{k-1}$, there is a unit $u\equiv1\pmod{p^{k-1}}$ with $\chi(u)\ne1$. For $k=1$, reduction is to the unit group modulo one. If $p\mid a$, then $a(u-1)\equiv0\pmod q$, so multiplication of the summation variable by $u$ leaves its exponential factor unchanged. It follows that $\widehat\chi(a)=\chi(u)\widehat\chi(a)$, and therefore $\widehat\chi(a)=0$. Also $\chi(a)=0$. This proves the formula at every nonunit as well as every unit, including $a=0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
