<h1 id="7d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Cauchy theorem for groups](../../../../../../cauchy-theorem-for-groups.md) says that if a prime $p$ divides $|G|$, then $G$ contains an element of order $p$.

Consider

$$
X=\{(x_1,\ldots,x_p)\in G^p:x_1x_2\cdots x_p=1\}.
$$

The first $p-1$ entries determine the last, so $|X|=|G|^{p-1}$, which is divisible by $p$. Cyclic rotation acts on $X$: if the product is one, then

$$
x_2\cdots x_px_1=x_1^{-1}(x_1\cdots x_p)x_1=1.
$$

Every orbit has size one or $p$. The fixed points are exactly the constant tuples $(x,\ldots,x)$ satisfying $x^p=1$. Since $|X|\equiv0\pmod p$, the number of fixed points is divisible by $p$. The identity supplies one, so there is a nonidentity $x$ with $x^p=1$. Its order divides the prime $p$ and is not one, hence is $p$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7D](../../7d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
