<h1 id="19g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The finite-dimensional [inner product space](../../../../../../inner-product-space.md) has the [orthogonal decomposition](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md) $U=W\oplus W^\perp$. Define $\tau(w+z)=w$ for $w\in W$, $z\in W^\perp$. This is a [linear map](../../../../../../linear-map.md) with image $W$, satisfies $\tau^2=\tau$, and is self-adjoint by taking [inner products](../../../../../../inner-product.md) between decomposed vectors. Hence it is an [orthogonal projection](../../../../../../orthogonal-projection.md).

Any other [orthogonal projection](../../../../../../orthogonal-projection.md) with image $W$ has kernel $W^\perp$ by part (a); it is identity on $W$ by idempotence and zero on its kernel. Its values are therefore forced to agree with $\tau$, proving uniqueness.

If $\tau_2\tau_1=0$, every $w_1\in W_1$ has $w_1=\tau_1w_1$, so $\tau_2w_1=0$ and $w_1\in W_2^\perp$. Conversely, if $W_1\subset W_2^\perp$, every image $\tau_1u$ is killed by $\tau_2$. Therefore

$$
\boxed{\tau_2\circ\tau_1=0\quad\Longleftrightarrow\quad W_1\perp W_2.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19G](../../19g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
