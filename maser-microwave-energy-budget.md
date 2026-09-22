# Maser microwave energy budget

↑ **Parent:** [Maser oscillation threshold](maser-oscillation-threshold.md)

Multiplying the upper-level and [photon](photon.md) equations by $h\nu_0$ makes the cancellation of internal transfer visible:

$$
\frac{d}{dt}\bigl[h\nu_0(N_u+n)\bigr]
=h\nu_0F-\gamma h\nu_0N_u-\kappa_{\mathrm{int}}h\nu_0n-\kappa_{\mathrm{out}}h\nu_0n.
$$

Incoming excitation becomes unused excitation carried away, internal dissipation, useful output, or a change in stored [energy](energy-split.md). Translational [kinetic energy](kinetic-energy.md), the source's other internal states and preparation losses lie outside this two-level budget. The output cannot exceed the incoming excitation [power](power.md) $h\nu_0F$.

Choose $G=10^{-4}\,\mathrm{s^{-1}}$ per unit inversion, $\gamma=10^4\,\mathrm{s^{-1}}$, $\kappa_{\mathrm{int}}=\kappa_{\mathrm{out}}=10^6\,\mathrm{s^{-1}}$, and $F=4\times10^{14}\,\mathrm{s^{-1}}$. These are stipulated teaching parameters. Then $N_0=4\times10^{10}$, $F_{\mathrm{th}}=2\times10^{14}\,\mathrm{s^{-1}}$, $N_{\mathrm{ss}}=2\times10^{10}$ and $n_{\mathrm{ss}}=5\times10^7$. Using the rounded [ammonia inversion transition](ammonia-inversion-transition.md) [frequency](frequency.md), the loaded [quality factor](q-factor.md) is approximately $7.50\times10^4$. The incoming excitation [power](power.md) is $6.327\,\mathrm{nW}$: $4.745\,\mathrm{nW}$ leaves unused, $0.791\,\mathrm{nW}$ becomes internal dissipation and $0.791\,\mathrm{nW}$ is useful output, with rounding in these displayed values.

There is an instructive extraction optimum within this model. With the same $F$, $G$ and $\gamma$, put $\rho=\kappa_{\mathrm{out}}/\kappa_{\mathrm{int}}$ and $p=FG/(\gamma\kappa_{\mathrm{int}})=4$. For $0\leq\rho<p-1$,

$$
P_{\mathrm{out}}=\frac{h\nu_0\gamma\kappa_{\mathrm{int}}}{2G}
\frac{\rho(p-1-\rho)}{1+\rho}.
$$

Differentiation gives $\rho_{\mathrm{opt}}=\sqrt p-1=1$. At zero coupling no [power](power.md) is extracted; at $\rho=3$ the device reaches onset and the nonzero branch disappears. The optimum balances extraction against the inversion required to compensate that extraction. Equal residence rates and loss of molecular phase memory are simplifying assumptions; the calculated efficiency is not a universal bound for beam masers.

## ↑ Ancestors (8)

1. [Maser oscillation threshold](maser-oscillation-threshold.md)
2. [Maser cavity](maser-cavity.md)
3. [Ammonia maser](ammonia-maser.md)
4. [Maser](maser-split.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Maser oscillation threshold](maser-oscillation-threshold.md)
