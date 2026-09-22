<h1 id="24h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [isometry](../../../../../../isometry.md) preserves the [Levi-Civita connection](../../../../../../levi-civita-connection.md). To justify this, transport the connection on $X$ by $d\psi$. It is torsion-free and preserves the metric on $Y$, since $\psi$ preserves the metric and Lie brackets. These two properties characterize the [Levi-Civita connection](../../../../../../levi-civita-connection.md) uniquely: if two such connections differ by $A$, the tensor $a(U,V,W)=\langle A(U,V),W\rangle$ is symmetric in its first two arguments and antisymmetric in its last two. Cycling these symmetries yields $a=-a$, hence $A=0$. Therefore

$$
d\psi(\nabla^X_UV)=\nabla^Y_{d\psi U}(d\psi V).
$$

Applying this along $\gamma$ shows that the covariant acceleration of $\psi\circ\gamma$ is zero, so **an [isometry](../../../../../../isometry.md) carries affinely parametrized [geodesics](../../../../../../geodesic.md) to [geodesics](../../../../../../geodesic.md)**.

The same identity and the definition $R(U,V)W=\nabla_U\nabla_VW-\nabla_V\nabla_UW-\nabla_{[U,V]}W$ show that $d\psi$ intertwines the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md). If $e_1,e_2$ is an [orthonormal](../../../../../../orthonormal-set.md) tangent basis, its image is [orthonormal](../../../../../../orthonormal-set.md) and

$$
K_Y(\psi(p))=\langle R_Y(d\psi e_1,d\psi e_2)d\psi e_2,d\psi e_1\rangle
=\langle R_X(e_1,e_2)e_2,e_1\rangle=K_X(p).
$$

**Both proposed converses are false.** Take $X=Y=\mathbb R^2$ with the Euclidean metric and $\psi(x)=2x$. A [geodesic](../../../../../../geodesic.md) $p+tv$ maps to the [geodesic](../../../../../../geodesic.md) $2p+2tv$, and both [Gaussian curvatures](../../../../../../gaussian-curvature.md) vanish identically. Nevertheless $\psi$ multiplies lengths by two, so is not an [isometry](../../../../../../isometry.md). This one counterexample answers both unheaded continuation requests.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [24H](../../24h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
