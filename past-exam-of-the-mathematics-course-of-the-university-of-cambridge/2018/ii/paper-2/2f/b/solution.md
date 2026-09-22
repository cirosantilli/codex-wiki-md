<h1 id="2f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For part (a), fix $\mathbf x\in L$ and consider the line segment

$$
\mathbf y(t)=(1-t)\mathbf1+t\mathbf x,
\qquad 0\leq t\leq1.
$$

The [convex set](../../../../../../convex-set.md) $L$ contains this entire segment. For

$$
g(t)=\prod_{j=1}^n\bigl(1+t(x_j-1)\bigr)
$$

we have $g(0)=1$ and

$$
g'(0)=\sum_{j=1}^n(x_j-1)=\sum_{j=1}^nx_j-n.
$$

If $\sum_jx_j>n$, then $g(t)>1$ for all sufficiently small positive $t$, contradicting the hypothesis on $L$. Thus

$$
\boxed{\sum_{j=1}^nx_j\leq n.}
$$

For part (b), $K$ is compact, and the product of the coordinates is a [continuous function](../../../../../../continuous-function.md). The [extreme value theorem](../../../../../../extreme-value-theorem.md) therefore supplies $\mathbf u\in K$ maximizing that product. Assume every $u_j>0$ and apply part (a) to the convex set

$$
L=\left\{\left(\frac{x_1}{u_1},\ldots,\frac{x_n}{u_n}\right):\mathbf x\in K\right\}.
$$

It contains $\mathbf1$, and maximality of $\mathbf u$ makes every coordinate product at most one. Hence

$$
\boxed{\sum_{j=1}^n\frac{x_j}{u_j}\leq n\qquad(\mathbf x\in K).}
$$

If $\mathbf v$ is another maximizer, its coordinates are positive and $\prod_j(v_j/u_j)=1$. The [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) gives

$$
\frac1n\sum_j\frac{v_j}{u_j}\geq
\left(\prod_j\frac{v_j}{u_j}\right)^{1/n}=1,
$$

while the displayed inequality gives the reverse bound. Equality in the arithmetic-geometric mean inequality forces every $v_j/u_j=1$. Therefore **the maximizer $\mathbf u$ is unique**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2F](../../2f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
