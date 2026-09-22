<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For any [vector field](../../../../../../vector-field.md) $Y$, apply the [Leibniz rule](../../../../../../leibniz-rule.md) to the scalar $\omega(Y)$:

$$
\mathcal L_V(\omega_aY^a)
=(\mathcal L_V\omega)_aY^a+\omega_a(\mathcal L_VY)^a.
$$

Using $\mathcal L_VY=[V,Y]$ and expanding the [Lie bracket](../../../../../../lie-bracket.md) in a coordinate chart leaves

$$
\boxed{(\mathcal L_V\omega)_a
=V^b\nabla_b\omega_a+\omega_b\nabla_aV^b}.
$$

The connection terms cancel because the [Levi-Civita connection](../../../../../../levi-civita-connection.md) is torsion-free. Applying this formula to each slot of the [metric tensor](../../../../../../metric-tensor.md) and using [metric compatibility](../../../../../../metric-compatibility.md) gives

$$
\boxed{(\mathcal L_Vg)_{ab}=\nabla_aV_b+\nabla_bV_a}.
$$

Equivalently, one may prove both identities at a point in [normal coordinates](../../../../../../normal-coordinates.md); since both sides are tensors, the result then holds in every coordinate system.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
