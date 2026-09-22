<h1 id="11e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [algebraic integer](../../../../../../algebraic-integer.md) is a complex number satisfying a monic polynomial with integer coefficients. Let $f\in\mathbb Q[x]$ be the monic [minimal polynomial](../../../../../../minimal-polynomial.md) of $\alpha$. It is irreducible over $\mathbb Q$. If $H\in\mathbb Z[x]$ is a monic polynomial vanishing at $\alpha$, then $f$ divides $H$ over $\mathbb Q$. [Gauss lemma for polynomials](../../../../../../gauss-lemma-for-polynomials.md) implies that monic rational factors of a monic integer polynomial have integer coefficients. Thus $f\in\mathbb Z[x]$, and its irreducibility over $\mathbb Q$ implies irreducibility in $\mathbb Z[x]$.

For $h\in\mathbb Z[x]$ with $h(\alpha)=0$, division by the monic $f$ works in $\mathbb Z[x]$, giving $h=qf+r$ with $\deg r<\deg f$. Since $r(\alpha)=0$, minimality forces $r=0$. Conversely each multiple of $f$ vanishes at $\alpha$. Therefore

$$
\boxed{I=(f),\qquad\mathbb Z[\alpha]\cong\mathbb Z[x]/(f).}
$$

Writing $n=\deg f$, division by $f$ expresses every element uniquely as $a_0+a_1\alpha+\cdots+a_{n-1}\alpha^{n-1}$ with integer coefficients. A relation among these powers would be a nonzero vanishing polynomial of degree less than $n$. Hence **$1,\alpha,\ldots,\alpha^{n-1}$ form a [basis](../../../../../../basis.md) of the [free module](../../../../../../free-module.md) over $\mathbb Z$ $\mathbb Z[\alpha]$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11E](../../11e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
