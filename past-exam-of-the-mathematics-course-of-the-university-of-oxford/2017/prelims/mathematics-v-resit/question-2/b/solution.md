<h1 id="question-2/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

Write $\partial_i=\partial/\partial x_i$ and use $\times$ for the paper's wedge notation, which denotes the [cross product](../../../../../../cross-product.md). The given expression for the [curl](../../../../../../curl.md) and the [product rule](../../../../../../product-rule.md) give

$$
\nabla\times(\mathbf v\times\mathbf w)
=\sum_i\mathbf e_i\times\bigl((\partial_i\mathbf v)\times\mathbf w
+\mathbf v\times(\partial_i\mathbf w)\bigr).
$$

Apply the [vector triple product identity](../../../../../../vector-triple-product.md) $\mathbf a\times(\mathbf b\times\mathbf c)=\mathbf b(\mathbf a\cdot\mathbf c)-\mathbf c(\mathbf a\cdot\mathbf b)$ separately to the two terms:

$$
\begin{aligned}
\mathbf e_i\times((\partial_i\mathbf v)\times\mathbf w)
&=w_i\partial_i\mathbf v-\mathbf w\,\partial_i v_i,\\
\mathbf e_i\times(\mathbf v\times\partial_i\mathbf w)
&=\mathbf v\,\partial_i w_i-v_i\partial_i\mathbf w.
\end{aligned}
$$

Summing over the Cartesian [basis vectors](../../../../../../basis-vector.md) identifies the two [directional derivatives](../../../../../../directional-derivative.md) and the two [divergences](../../../../../../divergence.md):

$$
\boxed{\nabla\times(\mathbf v\times\mathbf w)
=(\mathbf w\cdot\nabla)\mathbf v+\mathbf v(\nabla\cdot\mathbf w)
-(\mathbf v\cdot\nabla)\mathbf w-\mathbf w(\nabla\cdot\mathbf v)}.
$$

Here, for example, $((\mathbf w\cdot\nabla)\mathbf v)_j=\sum_iw_i\partial_i v_j$. This proves the [curl of a cross product](../../../../../../curl-of-a-cross-product.md) directly from the formula supplied.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [Question 2](../../question-2.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
