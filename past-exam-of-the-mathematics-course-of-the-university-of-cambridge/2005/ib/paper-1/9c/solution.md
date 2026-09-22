<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Let $\dim V=n$ and $\dim W=k$. Extend a [basis](../../../../../basis.md) $w_1,\ldots,w_k$ of the [vector subspace](../../../../../vector-subspace.md) $W$ to $w_1,\ldots,w_n$ of $V$, and let $f_1,\ldots,f_n$ be its [dual basis](../../../../../dual-basis.md). Every [linear functional](../../../../../linear-functional.md) is uniquely $\sum_i c_i f_i$. It vanishes on $W$ exactly when $c_1=\cdots=c_k=0$. Thus the [annihilator of a vector subspace](../../../../../annihilator-of-a-vector-subspace.md) has [basis](../../../../../basis.md) $f_{k+1},\ldots,f_n$, and

$$
\boxed{\dim\alpha(W)=n-k}.
$$

To apply this to a [matrix](../../../../../matrix.md), regard its rows as elements of $(\mathbb R^n)^*$ and let $R$ be their linear span. Elementary invertible row and column operations reduce a rank-$r$ [matrix](../../../../../matrix.md) to a block identity $\operatorname{diag}(I_r,0)$, showing that $\dim R=r$. The equations require that every functional in $R$ vanish on $x$. The canonical identification $\mathbb R^n\cong((\mathbb R^n)^*)^*$ sends $x$ to evaluation $f\mapsto f(x)$: it is injective because coordinate functionals separate points, and is bijective by equal dimensions. Consequently the solution [vector space](../../../../../vector-space-split.md) is the annihilator of $R$ under this identification. The dimension formula just proved gives

$$
\boxed{\dim\ker A=n-r}.
$$

A [basis](../../../../../basis.md) of this [kernel](../../../../../kernel-of-a-linear-map.md) consists of exactly $n-r$ [linearly independent](../../../../../linear-independence.md) solutions, and every solution is their linear combination.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
