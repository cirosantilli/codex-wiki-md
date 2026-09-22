<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $|g|$ has a local maximum at $z_0$. If $g(z_0)=0$, the nonnegativity of the modulus forces $g=0$ throughout a neighbourhood, and the [identity theorem for holomorphic functions](../../../../../../../identity-theorem.md) makes it zero on that connected component.

If $g(z_0)\ne0$, take $c=2i/g(z_0)$. Then $cg(z_0)=2i$, and continuity gives a disk $D$ around $z_0$ on which $\Im(cg)>1$. This lies within the given half-plane for a branch of the [holomorphic logarithm](../../../../../../../holomorphic-logarithm.md). On $D$ define

$$
f=\operatorname{Log}(cg),\qquad\Re f=\log|cg|=\log|c|+\log|g|.
$$

Composition preserves holomorphy, and the real logarithm is strictly increasing, so $\Re f$ has a local maximum at $z_0$. Part (i) forces $f$ to be constant on the disk. Exponentiating gives $cg=e^f$, hence $g$ is constant there and, by the [identity theorem for holomorphic functions](../../../../../../../identity-theorem.md), on the whole connected component. Therefore

$$
\boxed{\text{A local maximum of }|g|\text{ forces }g\text{ to be constant on its connected component.}}
$$

This proves the [maximum modulus principle](../../../../../../../maximum-modulus-principle.md) by the requested logarithm argument. Multiplication by $c$ is what puts the image in the supplied logarithm branch; no global logarithm of $g$ is assumed.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
