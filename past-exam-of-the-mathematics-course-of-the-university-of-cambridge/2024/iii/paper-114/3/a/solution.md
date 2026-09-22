<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The standard [CW complex](../../../../../../cw-complex.md) structure on $\mathbb{CP}^n$ has one cell in every even dimension from $0$ to $2n$, and $\mathbb{CP}^k$ is its $2k$-skeleton. Collapsing that subcomplex leaves one zero-cell and one cell in each dimension $2i$ for $k+1\leq i\leq n$. All [cellular boundaries](../../../../../../cellular-boundary-formula.md) vanish, so

$$
\boxed{H^q(\mathbb{CP}^n/\mathbb{CP}^k;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&q=0\text{ or }q=2i,quad k+1\leq i\leq n,\\
0,&\text{otherwise}.
\end{cases}}
$$

Let $x\in H^2(\mathbb{CP}^n;\mathbb Z)$ be the usual generator. For $i>k$, choose $u_i$ whose pullback under the [quotient map](../../../../../../quotient-map.md) is $x^i$. Naturality of the [cup product](../../../../../../cup-product.md) and the [cohomology ring of complex projective space](../../../../../../cohomology-ring-of-complex-projective-space.md) give

$$
u_i u_j=\begin{cases}
u_{i+j},&i+j\leq n,\\
0,&i+j>n.
\end{cases}
$$

Together with the unit, this determines the ring; equivalently, its reduced part is the ideal $(x^{k+1})/(x^{n+1})$ with the inherited multiplication. This is the [cohomology ring of a collapsed projective subspace](../../../../../../cohomology-ring-of-a-collapsed-projective-subspace.md).

If $n=k+1$, the quotient has just a zero-cell and a $2n$-cell, so it is $S^{2n}$ and is a compact manifold. Conversely, suppose $n\geq k+2$ and the quotient is homotopy equivalent to a compact manifold. Its top cohomology is $\mathbb Z$, so that manifold must be closed, orientable, and $2n$-dimensional. But $H^{2n-2}\cong\mathbb Z$ while $H^2=0$, contradicting [Poincare duality](../../../../../../poincare-duality.md). Therefore

$$
\boxed{\mathbb{CP}^n/\mathbb{CP}^k\text{ is homotopy equivalent to a compact manifold exactly when }n=k+1.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
