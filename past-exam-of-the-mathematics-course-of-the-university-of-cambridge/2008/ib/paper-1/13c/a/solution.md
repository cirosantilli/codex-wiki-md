<h1 id="13c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $a=1/n$, so $0<a<1$, and write $I(a)=\int_0^\infty x^a/(1+x^2)\,dx$. Choose the [branch of the complex logarithm](../../../../../../branch-of-the-complex-logarithm.md) with $-\pi/2<\arg z<3\pi/2$, whose cut is the downward imaginary axis. Define $z^a=\exp(a\operatorname{Log}z)$ and integrate $z^a/(1+z^2)$ along the positively oriented upper semicircle, indented above zero. The straight pieces run from $-R$ to $-\varepsilon$ and from $\varepsilon$ to $R$; the small arc runs clockwise from argument $\pi$ to zero.

On the negative real axis $z^a=|z|^ae^{i\pi a}$, so the two straight pieces tend to $(1+e^{i\pi a})I(a)$. The outer arc is $O(R^{a-1})$ and the inner arc is $O(\varepsilon^{a+1})$, both tending to zero. The only enclosed [pole](../../../../../../pole.md) is $i$, with [residue](../../../../../../residue.md) $e^{i\pi a/2}/(2i)$. The [residue theorem](../../../../../../residue-theorem.md) therefore gives

$$
(1+e^{i\pi a})I(a)=\pi e^{i\pi a/2}.
$$

Using $1+e^{i\pi a}=2e^{i\pi a/2}\cos(\pi a/2)$ yields

$$
\boxed{I(1/n)=\frac{\pi}{2\cos(\pi/(2n))}.}
$$

The same bounds show convergence of the real integral at both zero and infinity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13C](../../13c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
