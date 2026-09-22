<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathcal Z_M^1$ be the [sheaf of closed holomorphic one-forms](../../../../../../sheaf-of-closed-holomorphic-one-forms.md), namely $\ker(\partial:\Omega_M^1\to\Omega_M^2)$. The local exactness proved in part (b) gives the [short exact sequence of sheaves](../../../../../../short-exact-sequence-of-sheaves.md)

$$
0\longrightarrow\underline{\mathbb C}\longrightarrow\mathcal O_M\xrightarrow{\partial}\mathcal Z_M^1\longrightarrow0.
$$

Its [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) begins

$$
H^0(M,\mathbb C)\longrightarrow H^0(M,\mathcal O_M)
\longrightarrow H^0(M,\mathcal Z_M^1)
\xrightarrow{\delta}H^1(M,\mathbb C)\longrightarrow H^1(M,\mathcal O_M).
$$

The first arrow is an isomorphism: on a compact [complex manifold](../../../../../../complex-manifold.md), a global [holomorphic function](../../../../../../holomorphic-function.md) is constant on each [connected component](../../../../../../connected-component.md), just as a global section of the [constant sheaf](../../../../../../constant-sheaf.md) is. Thus $\delta$ is injective. By part (c), every global [holomorphic differential form](../../../../../../holomorphic-differential-form.md) of degree one is closed, so $H^0(M,\mathcal Z_M^1)=H^0(M,\Omega_M^1)$.

Concretely, for a [holomorphic differential form](../../../../../../holomorphic-differential-form.md) of degree one choose local holomorphic primitives $f_i$. The connecting class $\delta(\alpha)$ is represented by the locally constant [Čech cocycle](../../../../../../cech-cocycle-condition.md) $f_j-f_i$ on overlaps. The following arrow is induced by the inclusion of the [constant sheaf](../../../../../../constant-sheaf.md) into the [sheaf of holomorphic functions](../../../../../../structure-sheaf-of-a-complex-manifold.md). Exactness is inherited from the long exact sequence, giving

$$
\boxed{0\longrightarrow H^0(M,\Omega_M^1)\xrightarrow{\delta}H^1(M,\mathbb C)
\longrightarrow H^1(M,\mathcal O_M).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
