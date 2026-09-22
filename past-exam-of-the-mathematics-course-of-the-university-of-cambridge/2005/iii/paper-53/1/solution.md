<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $t=\log\mu$ and use $\alpha_i=g_i^2/(4\pi)$. The [chain rule](../../../../../chain-rule.md) turns the [renormalization-group beta function](../../../../../beta-function-physics.md) into

$$
\frac{d\alpha_i}{dt}=\frac{g_i}{2\pi}\frac{dg_i}{dt}=\frac{\beta_i}{2\pi}\alpha_i^2,
\qquad \frac{d\alpha_i^{-1}}{dt}=-\frac{\beta_i}{2\pi}.
$$

Integrating gives the [one-loop inverse gauge coupling evolution](../../../../../one-loop-inverse-gauge-coupling-evolution.md)

$$
\boxed{\alpha_i^{-1}(\mu)=\alpha_i^{-1}(M_Z)-\frac{\beta_i}{2\pi}\log\frac\mu{M_Z}.}
$$

This expression applies over a range with unchanged active field content and in the perturbative regime. It uses $\log\mu$, not $\log\mu^2$.

For [gauge coupling unification](../../../../../gauge-coupling-unification.md), define the normalized inverse couplings $A_1=3/(5\alpha_1)$, $A_2=1/\alpha_2$, $A_3=1/\alpha_3$, and slopes $b_1=(3/5)\beta_1$, $b_2=\beta_2$, $b_3=\beta_3$. At the common scale each inverse coupling is $A_U$. With $L=\log(M_{\mathrm{GUT}}/M_Z)$,

$$
A_i(M_Z)=A_U+\frac{b_i}{2\pi}L.
$$

Subtract the equations for factors 1 and 2 to solve $L=2\pi(A_1-A_2)/(b_1-b_2)$, then insert this into the difference of factors 3 and 2:

$$
\boxed{\frac1{\alpha_3(M_Z)}=\frac1{\alpha_2(M_Z)}+
\frac{\beta_3-\beta_2}{(3/5)\beta_1-\beta_2}
\left[\frac3{5\alpha_1(M_Z)}-\frac1{\alpha_2(M_Z)}\right].}
$$

This [one-loop normalized hypercharge unification](../../../../../one-loop-normalized-hypercharge-unification.md) relation requires $b_1\ne b_2$. A scale above $M_Z$ also requires the inferred $L$ to be positive. If those two slopes coincide, unification instead requires $A_1=A_2$ and their difference cannot fix the scale.

In the convention $Q=T_3+Y$, one matter generation and one [Higgs doublet](../../../../../higgs-field.md) have the following [Standard Model representations](../../../../../standard-model-representation.md). [Spin](../../../../../spin.md) is in units of $\hbar$; L/R describe [chirality](../../../../../chirality-physics.md), not the [spin](../../../../../spin.md) projection. The $U(1)_Y$ entry is its [hypercharge](../../../../../hypercharge.md) eigenvalue, defining the one-dimensional [representation](../../../../../group-representation.md) $e^{iY\omega}$.

| Field | [Spin](../../../../../spin.md) | [Chirality](../../../../../chirality-physics.md) | $Y$ | $SU(2)_L$ | $SU(3)_c$ |
| --- | --- | --- | --- | --- | --- |
| $Q_L=(u_L,d_L)^T$ | $1/2$ | Left | $1/6$ | $\mathbf2$ | $\mathbf3$ |
| $u_R$ | $1/2$ | Right | $2/3$ | $\mathbf1$ | $\mathbf3$ |
| $d_R$ | $1/2$ | Right | $-1/3$ | $\mathbf1$ | $\mathbf3$ |
| $L_L=(\nu_{eL},e_L)^T$ | $1/2$ | Left | $-1/2$ | $\mathbf2$ | $\mathbf1$ |
| $e_R$ | $1/2$ | Right | $-1$ | $\mathbf1$ | $\mathbf1$ |
| $H=(H^+,H^0)^T$ | $0$ | Not applicable | $1/2$ | $\mathbf2$ | $\mathbf1$ |

There is no [right-handed neutrino](../../../../../right-handed-neutrino.md) in the minimal field content being counted. Right-handed matter can alternatively be written as left-handed charge-conjugate [Weyl fermions](../../../../../weyl-spinor.md), in conjugate colour [representations](../../../../../group-representation.md) with opposite [hypercharges](../../../../../hypercharge.md). The quadratic indices and squared charges in the beta coefficients are unchanged.

For $SU(3)$, one generation supplies two colour fundamentals from $Q_L$ and one each from $u_R,d_R$. With three generations there are $n_f=3(2+1+1)=12$ [Weyl fermions](../../../../../weyl-spinor.md) counted as fundamental copies, and no coloured scalar. Thus

$$
\beta_3=-\frac{11}{3}\,3+\frac13\,12=\boxed{-7}.
$$

For $SU(2)$, the three colours of $Q_L$ give three weak-doublet copies and $L_L$ gives one. There are $n_f=3(3+1)=12$ doublets across three generations and $n_s=1$ complex [Higgs doublet](../../../../../higgs-field.md), giving

$$
\beta_2=-\frac{11}{3}\,2+\frac13\,12+\frac16=\boxed{-\frac{19}{6}}.
$$

These are [spectator multiplicities in gauge beta functions](../../../../../spectator-multiplicities-in-gauge-beta-functions.md): the colour index multiplies the weak contribution, while the weak index multiplies the colour contribution. Each two-component fermion is counted once; it must not be counted again as a separate [antiparticle](../../../../../antiparticle.md).

For $U(1)_Y$, sum squared [hypercharges](../../../../../hypercharge.md) over all colour and weak components. One generation gives

$$
\sum_{f,\,\text{one generation}}Y_f^2
=6\left(\frac16\right)^2+3\left(\frac23\right)^2+3\left(-\frac13\right)^2+2\left(-\frac12\right)^2+(-1)^2=\frac{10}{3}.
$$

The two complex Higgs components give $\sum_sY_s^2=2(1/2)^2=1/2$. There is no Abelian gauge self-interaction contribution. Therefore

$$
\beta_1=\frac23\,3\,\frac{10}{3}+\frac13\,\frac12=\boxed{\frac{41}{6}},\qquad
\boxed{(\beta_1,\beta_2,\beta_3)=\left(\frac{41}{6},-\frac{19}{6},-7\right).}
$$

The Higgs is counted only once for the whole model, whereas the fermionic generation is repeated three times. These are the [Standard Model one-loop gauge coefficients](../../../../../standard-model-one-loop-gauge-coefficients.md) in the unnormalized [hypercharge](../../../../../hypercharge.md) convention. The grand-unified normalization instead has $b_1=41/10$. The ratio of slopes in the unification relation is $(\beta_3-\beta_2)/(b_1-\beta_2)=-115/218$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
