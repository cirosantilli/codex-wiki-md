<h1 id="6c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write a vector in the domain as $(u,v,w,t)^T$. The first and third equations defining the [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) imply $v=2\alpha u-2t$. Substitution into the second equation then gives

$$
2(\alpha-1)\bigl(t-(\alpha+1)u\bigr)=0.
$$

For $\alpha\ne1$, this forces $t=(\alpha+1)u$, $v=-2u$ and $w=3u$. Hence

$$
\boxed{\ker M_\alpha=\operatorname{span}\{(1,-2,3,\alpha+1)^T\},\qquad\operatorname{im}M_\alpha=\mathbb R^3\quad(\alpha\ne1).}
$$

The [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) has dimension one, so the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) gives rank three and proves the assertion about the [image of a linear map](../../../../../../image-of-a-linear-map.md). Alternatively, the minor formed from columns $2,3,4$ has [determinant](../../../../../../determinant.md) $2(\alpha-1)$, including a nonzero value at $\alpha=-1$.

For $\alpha=1$, the parameters $u,t$ are free and $v=2u-2t$, $w=-3u+3t$. Thus

$$
\boxed{\ker M_1=\operatorname{span}\{(1,2,-3,0)^T,(0,-2,3,1)^T\}.}
$$

The third row is the first row minus the second. The [image of a linear map](../../../../../../image-of-a-linear-map.md) is therefore contained in $y_1-y_2-y_3=0$. The first and third columns, $(1,2,-1)^T$ and $(1,0,1)^T$, are linearly independent, so the [matrix rank](../../../../../../matrix-rank.md) is two and this containment is equality:

$$
\boxed{\operatorname{im}M_1=\{y\in\mathbb R^3:y_1-y_2-y_3=0\}=\operatorname{span}\{(1,2,-1)^T,(1,0,1)^T\}.}
$$

This is the sole [kernel jump in a parameter-dependent linear map](../../../../../../kernel-jump-in-a-parameter-dependent-linear-map.md); there is no further exceptional case at $\alpha=-1$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6C](../../6c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
