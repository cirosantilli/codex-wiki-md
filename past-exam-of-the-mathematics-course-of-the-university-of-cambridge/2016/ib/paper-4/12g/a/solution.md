<h1 id="12g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Two [norms](../../../../../../norm.md) $N_1,N_2$ on the same vector space are [equivalent norms](../../../../../../equivalent-norms.md), or Lipschitz equivalent, if there are constants $0<c\leq C<\infty$ such that $cN_1(v)\leq N_2(v)\leq CN_1(v)$ for every $v$. The constants are uniform over the whole space.

Let $N$ be any [norm](../../../../../../norm.md) on $\mathbb R^n$. The [triangle inequality](../../../../../../triangle-inequality.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
N(x)\leq\sum_i|x_i|N(e_i)\leq\left(\sum_iN(e_i)^2\right)^{1/2}\|x\|_2=C\|x\|_2.
$$

The reverse triangle inequality then gives $|N(x)-N(y)|\leq C\|x-y\|_2$, so $N$ is Euclidean-continuous; this continuity was derived, rather than assumed. On the compact Euclidean unit sphere, $N$ attains a strictly positive minimum $c$, because it vanishes only at zero. Homogeneity yields

$$
\boxed{c\|x\|_2\leq N(x)\leq C\|x\|_2.}
$$

Finally a [linear map](../../../../../../linear-map.md) $A:\mathbb R^n\to\mathbb R^m$ satisfies $\|Ax\|_2\leq(\sum_{i,j}|a_{ij}|^2)^{1/2}\|x\|_2$, again by [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). The equivalence just proved transfers this bound to any norms on the source and target. Hence **every such linear map is continuous**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12G](../../12g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
