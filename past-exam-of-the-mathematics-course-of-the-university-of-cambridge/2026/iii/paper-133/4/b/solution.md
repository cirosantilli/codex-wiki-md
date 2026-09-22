<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Retain the $(\lambda,\varepsilon)$-quasi-isometry $f:X\to T$ and the [Morse lemma for quasi-geodesics](../../../../../../morse-lemma-for-quasi-geodesics.md) constant $R$. Given $x,y\in X$, let $m$ be the midpoint of a geodesic $[x,y]$. There is a point $z$ on the tree geodesic $[f(x),f(y)]$ with

$$
d_T(f(m),z)\leq R.
$$

For any continuous path $\alpha$ from $x$ to $y$, choose a partition fine enough that consecutive $\alpha(t_i)$ are at distance at most one. Consecutive images under $f$ are then at distance at most

$$
D=\lambda+\varepsilon.
$$

Removing $z$ separates $f(x)$ from $f(y)$ in the tree along their geodesic, so this finite $D$-chain must contain an element within $D$ of $z$. For the corresponding $t_i$,

$$
d_T(f(m),f(\alpha(t_i)))\leq R+D.
$$

The lower quasi-isometry inequality yields

$$
d_X(m,\alpha(t_i))
\leq\lambda(R+D+\varepsilon).
$$

This constant depends only on the chosen quasi-isometry, so every [quasi-tree](../../../../../../quasi-tree.md) has the [bottleneck property](../../../../../../bottleneck-property.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
