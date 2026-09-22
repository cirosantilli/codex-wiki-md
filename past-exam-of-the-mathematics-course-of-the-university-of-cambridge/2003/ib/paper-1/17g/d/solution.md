<h1 id="17g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Inversion permutes the nonzero residues excluding $-1$. Hence the result of part (c) changes the requested sum into

$$
\sum_{n=1}^{p-2}\left(\frac{n(n+1)}p\right)=\sum_{m=1}^{p-2}\left(\frac{m+1}p\right)=\sum_{j=2}^{p-1}\left(\frac jp\right).
$$

There are exactly $(p-1)/2$ nonzero squares: the map $x\mapsto x^2$ on nonzero residues identifies exactly the pairs $x,-x$, because $x^2=y^2$ implies $x=\pm y$ in the [finite field](../../../../../../finite-field.md). Thus there are equally many nonzero squares and nonsquares, and the [complete Legendre-symbol sum](../../../../../../complete-legendre-symbol-sum.md) is zero. Removing the $j=1$ term leaves

$$
\boxed{\sum_{n=1}^{p-2}\left(\frac{n(n+1)}p\right)=-1.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
