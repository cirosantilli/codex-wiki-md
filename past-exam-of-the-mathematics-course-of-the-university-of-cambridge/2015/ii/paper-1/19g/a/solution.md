<h1 id="19g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the convention that the [inner product](../../../../../../inner-product.md) is linear in its first argument. Set $a_n=\langle x,e_n\rangle$ and $P_Nx=\sum_{n\leq N}a_ne_n$. Orthogonality makes $P_Nx$ the nearest point in the finite span of the first $N$ basis vectors. Since an [orthonormal basis](../../../../../../orthonormal-basis.md) has dense linear span, for every $\epsilon>0$ a finite linear combination approximates $x$ within $\epsilon$. For all larger $N$, the nearest-point property gives $\|x-P_Nx\|<\epsilon$. Thus the series converges in $X$ to $x$ even without completeness. Taking [inner products](../../../../../../inner-product.md) with each $e_n$ proves uniqueness of its coefficients.

In the Hilbert-space case, [Parseval's identity](../../../../../../parseval-identity.md) gives $\sum|a_n|^2=\|x\|^2$. Completeness makes

$$
\boxed{Ux=\sum_{n=1}^\infty\langle x,e_n\rangle f_n}
$$

convergent. It is linear and preserves [inner products](../../../../../../inner-product.md) and norms, so bounded with norm one. Its inverse is the corresponding map sending $f_n$ to $e_n$; equivalently every coefficient sequence of a vector in the $f_n$ basis is also square-summable in the $e_n$ basis. Hence $U$ is surjective and **unitary**. Any bounded map agreeing on the $e_n$ agrees on their dense span and then on all of $X$, proving uniqueness.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19G](../../19g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
