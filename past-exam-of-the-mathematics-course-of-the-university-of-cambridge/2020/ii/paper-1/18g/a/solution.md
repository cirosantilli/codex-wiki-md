<h1 id="18g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [tower law for field extensions](../../../../../../tower-law-for-field-extensions.md) states that for finite [field extensions](../../../../../../field-extension.md)

$$
K\subseteq E\subseteq L,
$$

one has

$$
\boxed{[L:K]=[L:E][E:K]}.
$$

To prove it, let $(u_i)_{i=1}^m$ be a $K$-basis of $E$ and $(v_j)_{j=1}^n$ an $E$-basis of $L$. Every $x\in L$ can be written as $\sum_j a_jv_j$ with $a_j\in E$, and expanding each $a_j$ in the basis $(u_i)$ shows that the $mn$ products $u_iv_j$ span $L$ over $K$.

If

$$
\sum_{i,j}c_{ij}u_iv_j=0,\qquad c_{ij}\in K,
$$

then independence of the $v_j$ over $E$ gives $\sum_i c_{ij}u_i=0$ for every $j$, and independence of the $u_i$ over $K$ gives every $c_{ij}=0$. Thus $(u_iv_j)$ is a $K$-basis of $L$, proving the formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18G](../../18g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
