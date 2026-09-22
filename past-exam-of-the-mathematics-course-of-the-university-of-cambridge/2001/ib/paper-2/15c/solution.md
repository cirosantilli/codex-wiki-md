<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

The algebraic [dual space](../../../../../dual-space.md) is $V^*=\operatorname{Hom}_k(V,k)$, the vector space of linear functionals. For an ordered [basis](../../../../../basis.md) $v_1,\ldots,v_n$, define the [dual basis](../../../../../dual-basis.md) by $v^i(v_j)=\delta_{ij}$, equivalently $v^i(\sum_jx_jv_j)=x_i$. Every functional satisfies $\ell=\sum_i\ell(v_i)v^i$, proving spanning. Evaluating a zero linear combination on each $v_j$ forces every coefficient to vanish, proving independence.

For a [linear map](../../../../../linear-map.md) $\alpha:V\to W$, its [dual map](../../../../../transpose-of-a-linear-map.md) is $\alpha^*:W^*\to V^*$, $\alpha^*(\ell)=\ell\circ\alpha$. Suppose the matrix of $\alpha$ satisfies $\alpha(v_i)=\sum_jA_{ji}w_j$. Then

$$
\alpha^*(w^j)(v_i)=w^j(\alpha(v_i))=A_{ji}.
$$

These are the $i$th coordinates of $\alpha^*(w^j)$ in the dual basis, so **the dual matrix is** $\boxed{A^T}$. For complex vector spaces this is still an ordinary transpose, because the algebraic dual uses linear functionals, not conjugate-linear ones.

To prove equality of ranks directly, $\ker\alpha^*$ consists precisely of functionals on $W$ vanishing on $\operatorname{im}\alpha$, its [annihilator](../../../../../annihilator-ring-theory.md). A basis of the image extends to a basis of $W$; such functionals have zero values on the image basis and arbitrary values on the remaining $\dim W-\operatorname{rank}\alpha$ vectors. Thus $\dim\ker\alpha^*=\dim W-\operatorname{rank}\alpha$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives

$$
\boxed{\operatorname{rank}\alpha^*=\operatorname{rank}\alpha.}
$$

Finally, if $\alpha$ is invertible, for every $\ell\in V^*$ the two compositions give $(\ell\circ\alpha^{-1})\circ\alpha=\ell$ and $(\ell\circ\alpha)\circ\alpha^{-1}=\ell$. Hence the two dual maps are mutual inverses and

$$
\boxed{(\alpha^*)^{-1}=(\alpha^{-1})^*.}
$$

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
