<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Applying the preceding [derivative](../../../../../../derivative.md) identity repeatedly yields the [Bézier derivative control polygon](../../../../../../bezier-derivative-control-polygon.md) for every order:

$$
\boxed{P^{(r)}(t)=\frac{n!}{(n-r)!}\sum_{j=0}^{n-r}\Delta^rP_jB_j^{n-r}(t),\qquad0\le r\le n,}
$$

where the forward [finite difference](../../../../../../finite-difference-split.md) is $\Delta P_j=P_{j+1}-P_j$ and

$$
\Delta^rP_j=\sum_{k=0}^r(-1)^{r-k}\binom rkP_{j+k}.
$$

The induction step multiplies by the remaining degree $n-r$ and takes one more [finite difference](../../../../../../finite-difference-split.md). [Derivatives](../../../../../../derivative.md) above order $n$ vanish. In particular,

$$
P^{(r)}(0)=\frac{n!}{(n-r)!}\Delta^rP_0,\qquad P^{(r)}(1)=\frac{n!}{(n-r)!}\Delta^rP_{n-r}.
$$

If the actual parameter interval has length $h$ and $t$ is its normalized coordinate, [derivatives](../../../../../../derivative.md) in the original parameter acquire the additional factor $h^{-r}$. These formulas allow [derivative](../../../../../../derivative.md) evaluation and join tests using only the [control polygon](../../../../../../control-polygon.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
