<h1 id="37e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a point mass, $\Phi=-GM/r$, and part (b) gives

$$
h_{00}=\frac{2GM}{r}.
$$

The [linearized Ricci tensor and scalar](../../../../../../linearized-ricci-tensor-and-scalar.md) obey

$$
R=\partial_\mu\partial_\nu h^{\mu\nu}-\mathop{\Box}h.
$$

For a static perturbation with $h_{0i}=0$, this becomes

$$
R=\partial_i\partial_jh_{ij}+\nabla^2h_{00}-\nabla^2h_{ii}.
$$

Away from the source, $\nabla^2h_{00}=0$. For $h_{ij}=f(r)x_i x_j$, one has $h_{ii}=r^2f$, so the two supplied identities give

$$
R=
\left(r^2f''+8rf'+12f\right)
-\left(r^2f''+6rf'+6f\right)
=2rf'+6f.
$$

The vacuum trace equation $R=0$ therefore reduces to

$$
rf'+3f=0,
$$

whose general solution for $r>0$ is

$$
\boxed{f(r)=\frac{C}{r^3}}.
$$

The scalar equation alone leaves $C$ arbitrary. Imposing the remaining vacuum components $R_{ij}=0$ and matching the mass fixes $C=2GM$, as in the [linearized point-mass metric in radial Cartesian form](../../../../../../linearized-point-mass-metric-in-radial-cartesian-form.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [37E](../../37e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
