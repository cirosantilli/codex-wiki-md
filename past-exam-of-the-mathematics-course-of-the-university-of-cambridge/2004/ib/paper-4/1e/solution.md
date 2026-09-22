<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

For the given [orthonormal basis](../../../../../orthonormal-basis.md), the [orthogonal projection](../../../../../orthogonal-projection.md) is

$$
\boxed{\pi v=\sum_{j=1}^k\langle v,e_j\rangle e_j.}
$$

It belongs to $W$, and $\langle v-\pi v,e_j\rangle=0$ for every basis vector. Thus $v-\pi v\in W^\perp$. For any $w\in W$, decompose $v-w=(v-\pi v)+(\pi v-w)$. The summands are orthogonal, so the [Pythagorean theorem in an inner-product space](../../../../../pythagorean-theorem-in-an-inner-product-space.md) for the [inner product](../../../../../inner-product.md) gives

$$
\|v-w\|^2=\|v-\pi v\|^2+\|\pi v-w\|^2\geq\|v-\pi v\|^2.
$$

Equality holds exactly when $w=\pi v$. Hence **$\pi v$ is the unique closest point of $W$ to $v$**. This proves the minimizing property as well as the formula, including $W=\{0\}$ and $W=V$.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
