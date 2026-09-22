# Time-dependent neutral-B CP asymmetry

↑ **Parent:** [BABAR time-dependent CP violation experiment](babar-time-dependent-cp-violation-experiment.md)

With [CPT symmetry](cpt-symmetry.md), write the propagating states of [neutral meson mixing](neutral-meson-mixing.md) as $p|B^0\rangle\pm q|\bar B^0\rangle$, defining the coefficient ratio $q/p$. Let $\Delta m$ be their mass splitting and use units $\hbar=1$.

For rates $f_\pm$ tagged as $B^0,\bar B^0$ and $\Delta t=t_f-t_{\rm tag}$, neglect the [decay width](decay-width.md) difference and take $|q/p|=1$. Define

$$
\lambda_f=\frac qp\frac{\bar A_f}{A_f},\qquad
S=\frac{2\operatorname{Im}\lambda_f}{1+|\lambda_f|^2},\qquad
C=\frac{1-|\lambda_f|^2}{1+|\lambda_f|^2}.
$$

Here $A_f,\bar A_f$ are [decay amplitudes](decay-amplitude.md). The tagged asymmetry is $(f_+-f_-)/(f_++f_-)=S\sin(\Delta m\Delta t)-C\cos(\Delta m\Delta t)$ in this convention.[PDF p. 4, Eq. (1), tag signs and time convention](observation-of-cp-violation-in-the-b0-meson-system-by-babar-collaboration.md)

For a single [weak phase](weak-phase-cp-violation.md) in a [charmonium](charmonium.md)-[kaon](kaon.md) [CP eigenstate](cp-eigenstate.md) with eigenvalue $\eta_f$, $\lambda_f\simeq\eta_f e^{-2i\beta}$ gives $S=-\eta_f\sin2\beta$, $C\simeq0$, with

$$
\beta=\arg\!\left(-\frac{V_{cd}V_{cb}^*}{V_{td}V_{tb}^*}\right).
$$

This connects the [CKM unitarity triangle](ckm-unitarity-triangle.md) to [quantum interference](quantum-interference.md) between direct decay and decay after [neutral meson mixing](neutral-meson-mixing.md).[PDF p. 4, Eq. (1) and charmonium weak phase](observation-of-cp-violation-in-the-b0-meson-system-by-babar-collaboration.md)

For an independent teaching example choose $x=\Delta m\Delta t$, $\lambda_f=4i/3$ and an arbitrary common positive envelope $F(\Delta t)$. Then $S=24/25$, $C=-7/25$ and

$$
f_\pm=F(\Delta t)\left[1\pm\left(\frac{24}{25}\sin x+\frac7{25}\cos x\right)\right].
$$

Because $(24/25)^2+(7/25)^2=1$, both rates remain nonnegative. At $x=0$, the asymmetry is $7/25$; at $x=\pi/2$, it is $24/25$. These chosen values illustrate the sign convention and are not experimental estimates. More generally $S^2+C^2=1-[2\operatorname{Re}\lambda_f/(1+|\lambda_f|^2)]^2\le1$.

If a tag flips independently with probability $w$, exchanging $f_+$ and $f_-$ for that fraction of events gives $A_{\rm observed}=(1-2w)A_{\rm tag}$ by direct subtraction. The plotted toy choice $w=1/5$ reduces the amplitude to $3/5$ of its ideal value; at $w=1/2$ the tag contains no flavour information. Finite time resolution additionally averages over nearby oscillation phases. Extracting a [weak phase](weak-phase-cp-violation.md) consequently requires calibrated readout as well as a [CKM matrix](cabibbo-kobayashi-maskawa-matrix.md) prediction.

## ↑ Ancestors (8)

1. [BABAR time-dependent CP violation experiment](babar-time-dependent-cp-violation-experiment.md)
2. [Cabibbo-Kobayashi-Maskawa matrix](cabibbo-kobayashi-maskawa-matrix.md)
3. [Standard Model fermion](standard-model-fermion.md)
4. [Standard Model](standard-model-split.md)
5. [Quantum field theory](quantum-field-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [BABAR time-dependent CP violation experiment](babar-time-dependent-cp-violation-experiment.md)
