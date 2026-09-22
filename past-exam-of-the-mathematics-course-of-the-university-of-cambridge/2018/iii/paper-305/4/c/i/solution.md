<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [massless collinear parton approximation](../../../../../../../massless-collinear-parton-approximation.md) in a high-energy frame: $P^2=0$, $k=\xi P$, and $k'=\xi P+q$ with $k'^2=0$. This neglects target-mass corrections to the [parton model](../../../../../../../parton-model.md); it does not literally set a stationary massive target to a massless particle in the earlier flux formula.

For a [quark](../../../../../../../quark.md) of dimensionless charge $Q_f$, the electromagnetic [vector current](../../../../../../../vector-current.md) [matrix element](../../../../../../../matrix-element.md) is $Q_f\bar u(k')\gamma^\mu u(k)$. The [spin average](../../../../../../../spin-average.md) and [gamma-matrix trace](../../../../../../../gamma-matrix-trace.md) give

$$
\frac12\sum_{\rm spins}J^\mu J^{\nu *}=2Q_f^2\left(k^\mu k'^\nu+k^\nu k'^\mu-g^{\mu\nu}k\cdot k'\right).
$$

Integrating the three-momentum [Dirac delta function](../../../../../../../dirac-delta-function.md) in the [parton](../../../../../../../parton.md) [hadronic tensor](../../../../../../../hadronic-tensor.md) leaves

$$
\widetilde W^{\mu\nu}=\frac{\delta(q^0+\xi E_P-E_{k'})}{2\xi E_{k'}}\left(k^\mu k'^\nu+k^\nu k'^\mu-g^{\mu\nu}k\cdot k'\right).
$$

Since $k\cdot k'=\xi\nu$, this is

$$
\widetilde W^{\mu\nu}=\frac{\delta(q^0+\xi E_P-E_{k'})}{E_{k'}}\left[\xi P^\mu P^\nu+\frac12(P^\mu q^\nu+q^\mu P^\nu)-\frac\nu2g^{\mu\nu}\right].
$$

For the massless [Electron](../../../../../../../electron.md) momenta, $p^2=p'^2=0$ and $q=p-p'$. Substitution into the [leptonic tensor](../../../../../../../leptonic-tensor.md) gives

$$
q^\mu L_{\mu\nu}=4\left[-(p\cdot p')p'_\nu+(p\cdot p')p_\nu-(p\cdot p')(p_\nu-p'_\nu)\right]=0,
$$

and likewise $q^\nu L_{\mu\nu}=0$. These [Ward identities](../../../../../../../ward-identity.md) eliminate every term with an exposed $q$ index in the contraction. Therefore

$$
\boxed{\widetilde W^{\mu\nu}\doteq\frac{\delta(q^0+\xi E_P-E_{k'})}{E_{k'}}\left[\xi P^\mu P^\nu-\frac{\nu}{2}g^{\mu\nu}\right].}
$$

Here $\doteq$ means equality **after contraction with the [leptonic tensor](../../../../../../../leptonic-tensor.md)**. The shortened tensor is not itself conserved; the omitted terms restore [current conservation](../../../../../../../conserved-current.md) in the full [hadronic tensor](../../../../../../../hadronic-tensor.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 305](../../../../paper-305-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
