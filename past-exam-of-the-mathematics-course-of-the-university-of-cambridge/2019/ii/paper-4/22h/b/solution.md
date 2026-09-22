<h1 id="22h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $T$ is invertible, the [bounded inverse theorem](../../../../../../bounded-inverse-theorem.md) makes $T^{-1}$ bounded, and

$$
\|Tx\|\geq\|T^{-1}\|^{-1}\|x\|.
$$

Moreover $T^*$ is invertible with inverse $(T^{-1})^*$, so the same argument shows that $T^*$ is bounded below.

Conversely, suppose

$$
\|Tx\|\geq c\|x\|,
\qquad
\|T^*x\|\geq d\|x\|
$$

for some $c,d>0$. The first bound makes $T$ injective. It also makes $\operatorname{ran}T$ closed: if $Tx_n$ is Cauchy, then $x_n$ is Cauchy, and continuity gives its limit in the range. The second bound gives $\ker T^*=\{0\}$. By [image-kernel orthogonality for an adjoint](../../../../../../image-kernel-orthogonality-for-an-adjoint.md),

$$
(\operatorname{ran}T)^\perp=\ker T^*=\{0\},
$$

so the range is dense. Being both closed and dense, it equals $H$. Thus $T$ is bijective, and the first lower bound gives $\|T^{-1}\|\leq c^{-1}$. Therefore

$$
\boxed{T\text{ is invertible}
\quad\Longleftrightarrow\quad
T\text{ and }T^*\text{ are bounded below}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22H](../../22h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
