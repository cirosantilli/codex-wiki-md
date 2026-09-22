<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose $k$ distinct ranks whose $u(i)$ values are the $k$ largest, resolving any tie arbitrarily, and take the union of their full levels. Along a strict [chain in a partially ordered set](../../../../../../chain-in-a-partially-ordered-set.md), cardinality strictly increases, so this [set family](../../../../../../set-family.md) is a [k-Sperner family](../../../../../../k-sperner-family.md). Its weight is the sum of the selected rank weights because a full level of rank $i$ has $\binom ni$ members. Thus the bound in the [weighted theorem for k-Sperner families](../../../../../../weighted-theorem-for-k-sperner-families.md) is always attained:

$$
\boxed{\mathcal A=\bigcup_{i\in I}X^{(i)},\qquad |I|=k,\qquad w(\mathcal A)=\sum_{j=1}^k u_{(j)}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
