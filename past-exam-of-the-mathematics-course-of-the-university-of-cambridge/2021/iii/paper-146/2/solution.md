<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [almost complex structure](../../../../../almost-complex-manifold.md) $J$ on $(M,\omega_M)$ is a [compatible almost complex structure](../../../../../compatible-almost-complex-structure.md) when $J^2=-I$, $\omega_M(Ju,Jv)=\omega_M(u,v)$, and

$$
g_J(u,v)=\omega_M(u,Jv)
$$

is a positive-definite [inner product](../../../../../inner-product.md). To prove existence, choose any [Riemannian metric](../../../../../riemannian-metric.md) $h$ and define $A$ by $\omega_M(u,v)=h(Au,v)$. The [metric construction of a compatible almost complex structure](../../../../../metric-construction-of-a-compatible-almost-complex-structure.md)

$$
J=A(-A^2)^{-1/2}
$$

is smooth and compatible, so the space is nonempty.

Identify the compact symplectic manifold $N$ with its image under the [symplectic embedding](../../../../../symplectic-embedding.md). Along $N$ there is a symplectic splitting

$$
TM|_N=TN\oplus(TN)^{\omega_M}.
$$

Choose compatible almost complex structures on both summands and take their direct sum. Its associated metric makes the two summands orthogonal. Extend this metric from the closed submanifold $N$ to all of $M$ using a [partition of unity](../../../../../partition-of-unity.md), and apply the metric construction again. Along $N$ it recovers the prescribed direct sum, so the resulting global compatible $J$ satisfies $J(TN)=TN$. This is the [relative extension of a compatible almost complex structure](../../../../../relative-extension-of-a-compatible-almost-complex-structure.md).

For the two compact complex curves, use the supplied holomorphic coordinates at their transverse intersection. There $C_1\cup C_2$ is $\{xy=0\}$. Replace it in a small ball by the complex annulus $\{xy=\epsilon\}$ and use a cutoff in a surrounding annulus to rejoin the unchanged curves. For sufficiently small nonzero $\epsilon$, the result is an embedded symplectic surface $\Sigma$. This local replacement is a bordism between the old and new cycles, so

$$
[\Sigma]=[C_1]+[C_2]\in H_2(X;\mathbb Z).
$$

This is the [symplectic smoothing of a positive transverse node](../../../../../symplectic-smoothing-of-a-positive-transverse-node.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 146](../../paper-146-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
