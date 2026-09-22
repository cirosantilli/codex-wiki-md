<h1 id="17b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose that an $(n+1)$-node [quadrature rule](../../../../../../quadrature-rule.md) were exact on $\mathcal P_{2n+2}$. The nodal polynomial $Q_{n+1}$ has degree $n+1$, so $Q_{n+1}^2\in\mathcal P_{2n+2}$. At every node it vanishes, and hence

$$
I_n(Q_{n+1}^2)=0.
$$

But $Q_{n+1}^2$ is a nonzero nonnegative [polynomial](../../../../../../polynomial-split.md), and the weight function is positive on $(a,b)$. Therefore

$$
I(Q_{n+1}^2)=\int_a^bQ_{n+1}(x)^2w(x)\,dx>0,
$$

a contradiction. This is the [degree ceiling for quadrature exactness](../../../../../../degree-ceiling-for-quadrature-exactness.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17B](../../17b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
