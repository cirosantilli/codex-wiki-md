<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use $t_\mu=(1,-1,-1,-1)_\mu$ without summing in individual component transformations. The [Dirac current](../../../../../../dirac-current.md) transforms as

$$
\hat T(\bar\psi\gamma^\mu\psi)(x)\hat T^{-1}=t_\mu(\bar\psi\gamma^\mu\psi)(x_T).
$$

Since the coupling is real, invariance of its contraction fixes the [time reversal of an electromagnetic gauge field](../../../../../../time-reversal-of-an-electromagnetic-gauge-field.md):

$$
\boxed{\hat T A_0(x)\hat T^{-1}=A_0(x_T),\qquad \hat T A_i(x)\hat T^{-1}=-A_i(x_T).}
$$

These equations use a compatible gauge; an additional pure [gauge transformation](../../../../../../gauge-transformation.md) would not change the [gauge field strength](../../../../../../gauge-field-strength.md).

Coordinate differentiation at $x_T$ introduces $r_\mu=-t_\mu$, because the time coordinate is reversed and the spatial coordinates are unchanged. Hence

$$
\hat T F_{\mu\nu}(x)\hat T^{-1}=-t_\mu t_\nu F_{\mu\nu}(x_T),\qquad B^{-1}\sigma^{\mu\nu*}B=-t_\mu t_\nu\sigma^{\mu\nu}.
$$

Thus the [electric field](../../../../../../electric-field.md) is even and the [magnetic field](../../../../../../magnetic-field.md) is odd. The [chirality matrix](../../../../../../chirality-matrix.md) is even by part (a). The two tensor signs cancel in the dipole contraction, but [antiunitarity](../../../../../../antiunitary-operator.md) conjugates its explicit $i$. Therefore the [time-reversal parity of a fermion electric dipole operator](../../../../../../time-reversal-parity-of-a-fermion-electric-dipole-operator.md) is

$$
\boxed{\hat T\mathcal L_{\mathrm{EDM}}(x)\hat T^{-1}=-\mathcal L_{\mathrm{EDM}}(x_T).}
$$

It is a [time-reversal symmetry](../../../../../../t-symmetry.md) violating interaction, and, under the usual local relativistic [quantum field theory](../../../../../../quantum-field-theory-split.md) hypotheses of the [CPT theorem](../../../../../../cpt-theorem.md), it violates [CP symmetry](../../../../../../cp-symmetry.md). A nonzero coefficient is absent from the renormalizable tree-level [Standard Model](../../../../../../standard-model-split.md) [Lagrangian](../../../../../../lagrangian.md): the broken-phase [fermion electric dipole moment operator](../../../../../../fermion-electric-dipole-moment-operator.md) has [mass dimension](../../../../../../mass-dimension.md) five, and its electroweak-invariant completion requires a [Higgs field](../../../../../../higgs-field.md) and has dimension six. However, **it can arise as a radiatively induced effective interaction in the Standard Model**, whose [CKM matrix](../../../../../../cabibbo-kobayashi-maskawa-matrix.md) contains a [CP-violating phase](../../../../../../cp-violating-phase.md). It is not forbidden to all orders. An explicit primary calculation of quark dipoles is [Czarnecki and Krause's Standard Model calculation](https://arxiv.org/abs/hep-ph/9704355).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
