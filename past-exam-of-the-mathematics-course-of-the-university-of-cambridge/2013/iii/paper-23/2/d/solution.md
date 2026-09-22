<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a [nonprincipal Dirichlet character](../../../../../../nonprincipal-dirichlet-character.md), complete periods sum to zero, so its partial sums are bounded by $q$. [Partial summation](../../../../../../abel-s-summation-formula.md) at $X=q(1+t)$ yields

$$
L(1-it,\overline\chi)=\sum_{n\le X}\frac{\overline\chi(n)}{n^{1-it}}+O\left(\frac{q(1+t)}X\right).
$$

The head is bounded by $1+\log X$, hence $|L(1-it,\overline\chi)|\ll\log(q+t)$. The completed [functional equation](../../../../../../functional-equation.md) gives

$$
|L(it,\chi)|=\left(\frac q\pi\right)^{1/2}
\left|\frac{\Gamma((1-it)/2)}{\Gamma(it/2)}\right|,|L(1-it,\overline\chi)|.
$$

The stated gamma bounds make the ratio $O(t^{1/2})$: their exponential factors cancel, and their powers differ by $1/2$. Apply them directly for $t\ge4$; the compact interval $2\le t\le4$ is absorbed into the constant. Therefore

$$
\boxed{|L(it,\chi)|\ll\sqrt{qt}\,\log(q+t).}
$$

For the conductor-one principal case, Euler summation for zeta at $1-it$, truncated at $X=t^2$, gives a harmonic-size head, a [pole](../../../../../../pole.md) term of size $1/t$, and remainder $O((1+t)/X)$. It gives the same $O(\log t)$ bound before applying the zeta [functional equation](../../../../../../functional-equation.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
