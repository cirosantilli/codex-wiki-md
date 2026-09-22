<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [tree-level Feynman diagram](../../../../../../tree-level-feynman-diagram.md) contains one [weak charged current](../../../../../../charged-current.md) vertex. Fermion arrows point along fermion-number flow, so the outgoing [antiquark](../../../../../../antiquark.md) arrow points toward the vertex.

<a id="3/b/image-tree-level-w-plus-decay-into-an-outgoing-quark-and-antiquark-with-fermion-flow-arrows"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-305-w-decay.png)

**[Figure 1](#3/b/image-tree-level-w-plus-decay-into-an-outgoing-quark-and-antiquark-with-fermion-flow-arrows). Tree-level W-plus decay into an outgoing quark and antiquark with fermion-flow arrows**.

For one fixed matching color, the [scattering amplitude](../../../../../../scattering-amplitude.md) is

$$
\mathcal M=\frac{g}{2\sqrt2}V_{qq'}\epsilon_\mu(p)\bar u(k)\gamma^\mu(1-\gamma^5)v(k').
$$

An overall phase from the vertex has no effect on the width. The [fermion spin sums](../../../../../../fermion-spin-sum.md) give $\sum u\bar u=\not k$, $\sum v\bar v=\not k'$ in the massless approximation. For the three initial polarizations, use a [spin average](../../../../../../spin-average.md) of $1/3$. The [gamma matrix trace identities](../../../../../../gamma-matrix-trace-identities.md) give

$$
T^{\mu\nu}=\operatorname{Tr}\left[\not k\gamma^\mu(1-\gamma^5)\not k'\gamma^\nu(1-\gamma^5)\right]
=8\left(k^\mu k'^\nu+k^\nu k'^\mu-g^{\mu\nu}k\cdot k'+i\epsilon^{\mu\nu\rho\sigma}k_\rho k'_\sigma\right).
$$

The sign of the last term follows the PDF's $\gamma^5$ convention and does not affect this decay: the polarization sum is symmetric. Since $p=k+k'$ and the daughter masses vanish, $p_\mu T^{\mu\nu}=0$ and $k\cdot k'=M_W^2/2$. Therefore

$$
\overline{|\mathcal M|^2}_{\text{one color}}
=\frac{g^2|V_{qq'}|^2}{24}\left(-g_{\mu\nu}+\frac{p_\mu p_\nu}{M_W^2}\right)T^{\mu\nu}
=\frac{g^2M_W^2}{3}|V_{qq'}|^2.
$$

In the rest frame, the two-body [Lorentz-invariant phase space](../../../../../../lorentz-invariant-phase-space.md) integrates to $1/(8\pi)$: after the spatial delta function sets $\mathbf k'=-\mathbf k$, its radial delta function fixes $|\mathbf k|=M_W/2$. Explicitly,

$$
\int d\Phi_2=\frac{1}{16\pi^2}\int d\Omega\int_0^\infty dk\,\delta(M_W-2k)=\frac{1}{8\pi}.
$$

The decay formula consequently gives

$$
\Gamma_{\text{one color}}=\frac{\overline{|\mathcal M|^2}}{16\pi M_W}
=\frac{g^2M_W}{48\pi}|V_{qq'}|^2
=\boxed{\frac{G_FM_W^3}{6\pi\sqrt2}|V_{qq'}|^2.}
$$

**This is the printed expression, interpreted for one color.** For a physical quark-flavor channel there are three orthogonal final color states. Their probabilities add; no initial color average is present for a colorless [W boson](../../../../../../w-boson.md). Thus

$$
\boxed{\Gamma_{W^+\to q\bar q'}=N_c\frac{G_FM_W^3}{6\pi\sqrt2}|V_{qq'}|^2,\qquad N_c=3.}
$$

The PDF's formula omits this color multiplicity if read as the ordinary inclusive flavor width. It is also the familiar normalization for a colorless lepton channel.

The six physically accessible [quark](../../../../../../quark.md) combinations are **$u\bar d,u\bar s,u\bar b,c\bar d,c\bar s,c\bar b$**. A real on-shell [W boson](../../../../../../w-boson.md) cannot produce a [top quark](../../../../../../top-quark.md); the massless approximation is applied to the accessible daughters and does not open a physically forbidden top channel. [CKM matrix](../../../../../../cabibbo-kobayashi-maskawa-matrix.md) unitarity gives $\sum_{q'=d,s,b}|V_{uq'}|^2=\sum_{q'=d,s,b}|V_{cq'}|^2=1$. Therefore the physical color-summed hadronic width at this order is

$$
\boxed{\Gamma_{\rm had}=\frac{G_FM_W^3}{\pi\sqrt2}.}
$$

If the printed one-color convention is retained for every channel, its sum is instead $G_FM_W^3/(3\pi\sqrt2)$. In the artificial theory where all three up-type flavors, including the top, are kinematically massless, there would be nine channels and the physical sum would be $9G_FM_W^3/(6\pi\sqrt2)$; that is not the on-shell Standard Model channel list.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
