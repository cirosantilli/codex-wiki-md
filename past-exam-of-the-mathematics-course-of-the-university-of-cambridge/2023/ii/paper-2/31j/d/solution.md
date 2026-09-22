<h1 id="31j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First fix an ordered tuple $(g_1,\ldots,g_m)\in\mathcal G^m$. On writing

$$
z(x)=(g_1(x),\ldots,g_m(x))\in\mathbb R^m,
$$

the resulting classifiers are $x\mapsto\operatorname{sgn}(\alpha^Tz(x))$. The [growth bound for homogeneous linear classifiers](../../../../../../growth-bound-for-homogeneous-linear-classifiers.md) in dimension $m$ gives at most $(n+1)^m$ label vectors on any $n$ sample points.

If $\mathcal G$ is finite, there are $|\mathcal G|^m$ ordered tuples of hidden functions. The [shattering coefficient of a union](../../../../../../shattering-coefficient-of-a-union.md) therefore gives

$$
\boxed{s(\mathcal H_{\mathcal F_2},n)
\leq(n+1)^m|\mathcal G|^m.}
$$

For an arbitrary $\mathcal G$, fix $x_{1:n}$. Choose one representative for every distinct vector in $\mathcal G(x_{1:n})$, obtaining a finite class $\mathcal G'$ with

$$
|\mathcal G'|=|\mathcal G(x_{1:n})|
\leq s(\mathcal G,n).
$$

Every $m$-tuple from $\mathcal G$ agrees on the sample with an $m$-tuple from $\mathcal G'$. The finite-class argument now gives

$$
|\mathcal H_{\mathcal F_2}(x_{1:n})|
\leq(n+1)^m s(\mathcal G,n)^m.
$$

Taking the supremum over $x_{1:n}$ proves the general [growth bound for signs of m-term linear combinations](../../../../../../growth-bound-for-signs-of-m-term-linear-combinations.md):

$$
\boxed{s(\mathcal H_{\mathcal F_2},n)
\leq(n+1)^m s(\mathcal G,n)^m.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [31J](../../31j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
