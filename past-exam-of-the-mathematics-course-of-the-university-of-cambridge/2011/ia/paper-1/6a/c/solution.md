<h1 id="6a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expanding the formula from part (a) in components gives $y_i=x_i+(\alpha-1)n_i n_jx_j$, with repeated indices summed. Hence the [matrix of a linear map](../../../../../../matrix-representation-of-a-linear-map.md) and its inverse, when $\alpha\ne0$, have entries

$$
\boxed{A_{ij}=\delta_{ij}+(\alpha-1)n_i n_j,\qquad
B_{ij}=\delta_{ij}+(\alpha^{-1}-1)n_i n_j.}
$$

Here $\delta_{ij}$ is the [Kronecker delta](../../../../../../kronecker-delta.md). To check the [matrix inverse](../../../../../../matrix-inverse.md), write $P=nn^T$; $P^2=P$ because $|n|=1$. Thus $A=(I-P)+\alpha P$ and $B=(I-P)+\alpha^{-1}P$, whose product is the [identity matrix](../../../../../../identity-matrix.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6A](../../6a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
