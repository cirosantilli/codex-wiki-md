<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

For a [linear map](../../../../../linear-map.md) $T:V\to W$, its rank is $\dim\operatorname{im}T$ and its nullity is $\dim\ker T$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) states that, when $V$ is finite-dimensional,

$$
\dim V=\dim\ker T+\dim\operatorname{im}T.
$$

To prove it, take a [basis](../../../../../basis.md) $v_1,\ldots,v_k$ of $\ker T$ and extend it to a [basis](../../../../../basis.md)

$$
v_1,\ldots,v_k,v_{k+1},\ldots,v_n
$$

of $V$. The [vectors](../../../../../vector.md) $Tv_{k+1},\ldots,Tv_n$ span $\operatorname{im}T$. They are also linearly independent: if $\sum_{j=k+1}^na_jTv_j=0$, then $\sum_{j=k+1}^na_jv_j\in\ker T$, and independence of the chosen [basis](../../../../../basis.md) forces every $a_j$ to vanish. Thus the rank is $n-k$ and the nullity is $k$.

For the given subspace, row reduction of the coefficient [matrix](../../../../../matrix.md) gives

$$
\begin{pmatrix}
1&0&3&0&43/3\\
0&1&3&0&-5/3\\
0&0&0&1&-11/3
\end{pmatrix}.
$$

Taking $x_3=s$ and $x_5=t$ therefore gives

$$
(x_1,x_2,x_3,x_4,x_5)
=s(-3,-3,1,0,0)+\frac t3(-43,5,0,11,3).
$$

Hence

$$
\boxed{\dim W=2},
\qquad
\boxed{\{(-3,-3,1,0,0),(-43,5,0,11,3)\}}
$$

is a [basis](../../../../../basis.md) of $W$.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
