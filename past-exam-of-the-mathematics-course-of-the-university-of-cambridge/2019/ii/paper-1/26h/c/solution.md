<h1 id="26h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose $Q\in SO(n+1)$ with $Qe_{n+1}=v$. Conjugation by $Q$ identifies

$$
S_v=\{R\in SO(n+1):Rv=v\}
$$

with

$$
\left\{
\begin{pmatrix}A&0\\0&1\end{pmatrix}:A\in SO(n)
\right\}.
$$

It follows that the [unit-vector stabilizer in a special orthogonal group](../../../../../../unit-vector-stabilizer-in-a-special-orthogonal-group.md) is an embedded submanifold diffeomorphic to $SO(n)$, and

$$
\boxed{\dim S_v=\frac{n(n-1)}2}.
$$

At $R\in S_v$, its tangent space is

$$
T_RS_v=\{RA:A^T=-A,\ Av=0\}.
$$

For any $v\ne w$, both $S_v$ and $S_w$ contain the identity. At the identity,

$$
T_IS_v=\{A\in\mathfrak{so}(n+1):Av=0\},
\qquad
T_IS_w=\{A\in\mathfrak{so}(n+1):Aw=0\}.
$$

Identify $\mathfrak{so}(n+1)$ with the exterior square $\Lambda^2\mathbb R^{n+1}$. The orthogonal complement of $T_IS_v=\Lambda^2(v^\perp)$ is $v\wedge v^\perp$. If $v$ and $w$ are linearly independent, the nonzero bivector $v\wedge w$ belongs to the orthogonal complements of both tangent spaces. Their sum is therefore a proper subspace of $T_ISO(n+1)$, so the intersection is not [transverse](../../../../../../transverse-intersection.md). If $w=-v$, then $S_w=S_v$, whose tangent space is proper, so they are again not transverse. Consequently

$$
\boxed{S_v\text{ and }S_w\text{ are never transverse when }v\ne w},
$$

as summarized by [distinct unit-vector stabilizers are not transverse](../../../../../../distinct-unit-vector-stabilizers-are-not-transverse.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26H](../../26h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
