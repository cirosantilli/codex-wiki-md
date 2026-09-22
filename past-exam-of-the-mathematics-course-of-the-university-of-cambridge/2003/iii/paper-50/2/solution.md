<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $0\leq\sigma<2\pi$. Variation of the conformal-gauge [action](../../../../../action.md), with periodic variations, gives $(\partial_\tau^2-\partial_\sigma^2)X^\mu=0$. Hence $X^\mu=X_R^\mu(\tau-\sigma)+X_L^\mu(\tau+\sigma)$. In an uncompactified direction, periodicity allows equal linear slopes and independent periodic parts. Expanding the periodic parts in a [Fourier series](../../../../../fourier-series-split.md) yields the [closed-string mode expansion](../../../../../closed-string-mode-expansion.md)

$$
X^\mu=x^\mu+\alpha'p^\mu\tau+i\sqrt{\frac{\alpha'}2}\sum_{m\ne0}\frac1m\left(\alpha_m^\mu e^{-im(\tau-\sigma)}+\widetilde\alpha_m^\mu e^{-im(\tau+\sigma)}\right).
$$

Here $\alpha_m$ labels the right-moving sector and $\widetilde\alpha_m$ the left-moving sector; exchanging the names is harmless if done consistently. Integration of the [canonical momentum](../../../../../canonical-momentum.md) density $(2\pi\alpha')^{-1}\dot X^\mu$ over the string gives $p^\mu$, fixing the zero-mode coefficient. Reality gives $\alpha_m^\dagger=\alpha_{-m}$ and the analogous relation for tildes, with $\alpha_0=\widetilde\alpha_0=\sqrt{\alpha'/2}\,p$.

The [closed-string physical-state Virasoro conditions](../../../../../closed-string-physical-state-virasoro-conditions.md) are

$$
(L_0-1)|\Psi\rangle=(\widetilde L_0-1)|\Psi\rangle=0,\qquad L_m|\Psi\rangle=\widetilde L_m|\Psi\rangle=0\quad(m>0),
$$

where $L_0=\alpha'p^2/4+N$ and $\widetilde L_0=\alpha'p^2/4+\widetilde N$. Thus [closed-string level matching](../../../../../closed-string-level-matching.md) gives $N=\widetilde N$, and $M^2=-p^2=4(N-1)/\alpha'$. **The massless level is $N=\widetilde N=1$.** Its general state is

$$
|\zeta;p\rangle=\zeta_{\mu\nu}\alpha_{-1}^\mu\widetilde\alpha_{-1}^\nu|0;p\rangle.
$$

The [string oscillator](../../../../../string-oscillator.md) commutators give $[L_m,\alpha_n^\mu]=-n\alpha_{m+n}^\mu$: the two terms obtained by commuting through the quadratic generator coincide and cancel its factor $1/2$. Therefore $L_1$ replaces $\alpha_{-1}^\mu$ by $\alpha_0^\mu$, while $L_{m\geq2}$ produces positive [string oscillators](../../../../../string-oscillator.md) that annihilate this level. The same holds independently for tildes. The complete polarization conditions are

$$
\boxed{p^2=0,\qquad p^\mu\zeta_{\mu\nu}=0,\qquad p^\nu\zeta_{\mu\nu}=0.}
$$

[Null string states](../../../../../null-string-state.md) identify $\zeta_{\mu\nu}$ with $\zeta_{\mu\nu}+p_\mu\lambda_\nu+\widetilde\lambda_\mu p_\nu$, with transverse $\lambda,\widetilde\lambda$. At nonzero [momentum](../../../../../momentum.md) this leaves $24\cdot24=576$ physical polarizations. Their symmetric traceless, antisymmetric and transverse-trace parts are the [graviton](../../../../../graviton.md), [Kalb–Ramond field](../../../../../kalb-ramond-field.md) and [dilaton](../../../../../dilaton.md).

The original PDF's condition $\alpha'p^2=4$ is inconsistent with calling the displayed excited states massless. It is the on-shell condition of the [string oscillator](../../../../../string-oscillator.md) vacuum as a physical [tachyon](../../../../../tachyon.md). For the level-one state, that value would give $L_0=\widetilde L_0=2$, violating the physical conditions. The ket $|0;p\rangle$ used as the basis for a massless excitation must instead carry the excitation's [momentum](../../../../../momentum.md) $p^2=0$; by itself it is then not an on-shell physical vacuum state.

For the compact coordinate, $X^1(\tau,\sigma+2\pi)=X^1(\tau,\sigma)+2\pi wR$, $w\in\mathbb Z$. Its [momentum](../../../../../momentum.md) is $n/R$, $n\in\mathbb Z$, since the centre-of-mass wavefunction is single-valued on the circle. Thus its zero modes become

$$
X^1=x^1+\alpha'\frac nR\tau+wR\sigma+\text{the same periodic oscillator sum},
$$

with

$$
p_R=\frac nR-\frac{wR}{\alpha'},\qquad p_L=\frac nR+\frac{wR}{\alpha'},\qquad \alpha_0^1=\sqrt{\frac{\alpha'}2}p_R,\quad\widetilde\alpha_0^1=\sqrt{\frac{\alpha'}2}p_L.
$$

These are [momentum and winding modes](../../../../../momentum-and-winding-modes.md). Let $k$ be the 25-dimensional noncompact [momentum](../../../../../momentum.md) and $M^2=-k^2$. The two zero-mode constraints now give

$$
M^2=p_R^2+\frac4{\alpha'}(N-1)=p_L^2+\frac4{\alpha'}(\widetilde N-1).
$$

Their difference and average give, respectively,

$$
\widetilde N-N+nw=0,\qquad M^2=\frac{n^2}{R^2}+\frac{w^2R^2}{\alpha'^2}+\frac2{\alpha'}(N+\widetilde N-2).
$$

This also displays [T-duality](../../../../../t-duality.md) $R\leftrightarrow\alpha'/R$, $n\leftrightarrow w$, with one chiral [momentum](../../../../../momentum.md) reversed.

At a generic radius, the massless solutions are only $n=w=0$, $N=\widetilde N=1$. Their fields in 25 dimensions are a [graviton](../../../../../graviton.md) (275 polarizations), antisymmetric two-form (253), [dilaton](../../../../../dilaton.md) (one), two abelian [vectors](../../../../../vector.md) from $G_{a1}$ and $B_{a1}$ (23 each), and the radius scalar (one). Hence **the generic massless spectrum has $275+253+1+46+1=576$ polarizations**, with [gauge group](../../../../../gauge-group.md) $U(1)_L\times U(1)_R$. Here generic excludes isolated radii where [exceptional massless ground states of a bosonic circle](../../../../../exceptional-massless-ground-states-of-a-bosonic-circle.md) occur. Indeed $N=\widetilde N=0$ forces $nw=0$, and becomes massless at $R=|n|\sqrt{\alpha'}/2$ or $R=2\sqrt{\alpha'}/|w|$. These additional thresholds matter in the bosonic theory.

At the [self-dual circle](../../../../../self-dual-circle-compactification.md) $R=\sqrt{\alpha'}$, masslessness and level matching read

$$
n^2+w^2+2(N+\widetilde N-2)=0,\qquad\widetilde N-N+nw=0.
$$

Since $N,\widetilde N\geq0$, their sum is at most two. For sum two, $n=w=0$ and level matching gives the ordinary $(1,1)$ family. For sum one the four possibilities are

$$
(N,\widetilde N;n,w)=(1,0;1,1),\ (1,0;-1,-1),\ (0,1;1,-1),\ (0,1;-1,1).
$$

They have one right-moving $\alpha_{-1}$ or one left-moving $\widetilde\alpha_{-1}$ excitation, as their levels specify. Each family has 24 physical polarizations: a 25-dimensional [vector](../../../../../vector.md) with 23 polarizations and one compact-oscillator scalar. Thus these families add 96 states.

For sum zero, level matching forces $nw=0$, while the mass equation requires $n^2+w^2=4$. It gives four additional scalar states with charges **$(\pm2,0)$ and $(0,\pm2)$**, without any [string oscillators](../../../../../string-oscillator.md). They must not be omitted. The [massless spectrum at the bosonic self-dual circle](../../../../../massless-spectrum-at-the-bosonic-self-dual-circle.md) therefore has **100 additional polarizations, 676 in total**. The four new [vector](../../../../../vector.md) fields enhance the [gauge group](../../../../../gauge-group.md) to $SU(2)_L\times SU(2)_R$. Including the original radius scalar, the nine non-dilaton scalars form its $(3,3)$ representation. Equivalently, the full count is $275+253+1+6\cdot23+9=676$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
