# Neutral-kaon CP impurity and two-pion decay

↑ **Parent:** [CP violation](cp-violation.md)

Use the [kaon CP eigenstates](kaon-cp-eigenstates.md) convention $CP|K^0\rangle=-|\bar K^0\rangle$, matching [kaon CP mixing parameter](kaon-cp-mixing-parameter.md). Then $|K_1\rangle=(|K^0\rangle-|\bar K^0\rangle)/\sqrt2$ is [CP](cp-symmetry.md) even, while $|K_2\rangle=(|K^0\rangle+|\bar K^0\rangle)/\sqrt2$ is [CP](cp-symmetry.md) odd. With [CPT symmetry](cpt-symmetry.md) and a common small mixing parameter, the physical states can be written

$$
|K_S\rangle=\frac{|K_1\rangle+\epsilon|K_2\rangle}{\sqrt{1+|\epsilon|^2}},\qquad
|K_L\rangle=\frac{|K_2\rangle+\epsilon|K_1\rangle}{\sqrt{1+|\epsilon|^2}}.
$$

Here $S,L$ mean short and long [mean lifetimes](mean-lifetime-physics.md); the [kaon CP mixing parameter](kaon-cp-mixing-parameter.md) $\epsilon$ depends on the flavor-state phase convention. A positive flavor-exchange convention instead makes the symmetric flavor combination [CP](cp-symmetry.md) even, as explained in [exchange-positive CP convention for neutral kaon mixing](exchange-positive-cp-convention-for-neutral-kaon-mixing.md). Mixing these conventions would reverse the interpretation of the written sums.

Why does the two-[pion](pion.md) final state test [CP symmetry](cp-symmetry.md)? A spin-zero [kaon](kaon.md) decaying into two spin-zero [pions](pion.md) has relative [orbital angular momentum](orbital-angular-momentum.md) $\ell=0$ by [angular momentum conservation](conservation-of-angular-momentum.md). Two negative [intrinsic parities](intrinsic-parity.md) multiply to plus, and $(-1)^\ell=1$. [Charge conjugation](charge-conjugation.md) exchanges $\pi^+$ and $\pi^-$; the $\ell=0$ state is even under this exchange. Hence this two-[pion](pion.md) state has [CP](cp-symmetry.md) [eigenvalue](eigenvalue.md) $+1$. If a decay transition operator $T$ preserves [CP symmetry](cp-symmetry.md), inserting [CP](cp-symmetry.md) on both sides of $\langle\pi\pi|T|K_2\rangle$ changes its sign without changing its value: that [decay amplitude](decay-amplitude.md) must vanish.

Assume for illustration that [CP violation](cp-violation.md) occurs only through the state admixture and the decay transition preserves [CP symmetry](cp-symmetry.md). Put $A_1=\langle\pi\pi|T|K_1\rangle$. Then

$$
A_L=\frac{\epsilon A_1}{\sqrt{1+|\epsilon|^2}},\qquad
A_S=\frac{A_1}{\sqrt{1+|\epsilon|^2}},\qquad
\eta_{\pi\pi}=\frac{A_L}{A_S}=\epsilon.
$$

Neglecting the tiny difference in two-body [Lorentz-invariant phase space](lorentz-invariant-phase-space.md) between the physical [masses](mass.md) gives $\Gamma_L^{\pi\pi}/\Gamma_S^{\pi\pi}\simeq|\epsilon|^2$. A [branching fraction](branching-fraction.md), however, divides a partial [decay width](decay-width.md) by the total [decay width](decay-width.md). With $\hbar=1$, $\tau_i=1/\Gamma_i$, so

$$
\frac{B_L^{\pi\pi}}{B_S^{\pi\pi}}
\simeq |\epsilon|^2\frac{\Gamma_S}{\Gamma_L}
=|\epsilon|^2\frac{\tau_L}{\tau_S}.
$$

For chosen values $|\epsilon|=0.01$ and $\tau_L/\tau_S=100$, the [branching fraction](branching-fraction.md) ratio is $0.01$, whereas the partial [decay width](decay-width.md) ratio is $0.0001$. This is original arithmetic, not a historical fit. The longer observation time amplifies the integrated fraction relative to the instantaneous partial [decay rate](decay-width.md).

## ↑ Ancestors (6)

1. [CP violation](cp-violation.md)
2. [Discrete symmetry in quantum field theory](discrete-symmetry-in-quantum-field-theory.md)
3. [Quantum field theory](quantum-field-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Kaon CP eigenstates](kaon-cp-eigenstates.md)
