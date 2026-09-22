<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

Put $A=\operatorname{im}\alpha$. The restriction $\beta|_A$ has image $\operatorname{im}(\beta\alpha)$ and kernel $A\cap\ker\beta$. By the [rank-nullity theorem](../../../../../rank-nullity-theorem.md),

$$
r(\beta\alpha)=r(\alpha)-\dim(A\cap\ker\beta).
$$

Since its image is contained in $\operatorname{im}\beta$, this proves the upper bound. Also $\dim(A\cap\ker\beta)\le\dim\ker\beta=\dim V-r(\beta)$, giving the [rank inequality for a composition](../../../../../rank-inequality-for-a-composition.md):

$$
\boxed{r(\alpha)+r(\beta)-\dim V\le r(\beta\alpha)\le\min(r(\alpha),r(\beta)).}
$$

Examples on $U=V=W=\mathbb R^2$ distinguish the inequalities. Taking $\alpha=\beta=I$ gives equality in both. Taking $\alpha=\operatorname{diag}(1,0)$ and $\beta=\operatorname{diag}(0,1)$ gives composition rank zero, strictly below the upper bound 1 and equal to the lower bound 0. Taking $\alpha=\beta=\operatorname{diag}(1,0)$ gives rank 1, strictly above the lower bound 0 and equal to the upper bound 1.

For the final [nilpotent linear map](../../../../../nilpotent-linear-map.md), repeated application of the lower bound gives $r(\alpha^k)\ge2n-2k$. Since $\alpha^n=\alpha^{n-k}\alpha^k=0$, another application gives

$$
0\ge r(\alpha^{n-k})+r(\alpha^k)-2n
\ge2k+r(\alpha^k)-2n.
$$

The two bounds coincide, yielding

$$
\boxed{r(\alpha^k)=2n-2k\quad(1\le k\le n-1).}
$$

In fact the same formula includes $k=0,n$. For $n=1$ the requested index range is empty and the assumptions force $\alpha=0$.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
