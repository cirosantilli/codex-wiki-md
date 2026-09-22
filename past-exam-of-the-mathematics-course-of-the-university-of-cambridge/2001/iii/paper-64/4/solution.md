<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Consider the [closed bosonic string](../../../../../closed-string.md) on a rectangular product of spatial circles with no background mixing between them. Let $Y^j$ have period $2\pi R_j$, take $0\le\sigma<2\pi$, and choose $Y_L(\tau+\sigma)$ to be the tilded oscillator sector. Closed-string topology permits

$$
Y^j(\tau,\sigma+2\pi)=Y^j(\tau,\sigma)+2\pi w_jR_j,\qquad w_j\in\mathbb Z.
$$

Single-valued center-of-mass wavefunctions give quantized momentum $p^j=n_j/R_j$, $n_j\in\mathbb Z$. These are the [momentum and winding modes](../../../../../momentum-and-winding-modes.md). The oscillator modes remain integer moded; the zero modes are split as

$$
Y^j=x^j+\frac{\alpha'}2[p_L^j(\tau+\sigma)+p_R^j(\tau-\sigma)]+\text{oscillators},\qquad
p_L^j=\frac{n_j}{R_j}+\frac{w_jR_j}{\alpha'},\quad
p_R^j=\frac{n_j}{R_j}-\frac{w_jR_j}{\alpha'}.
$$

The two intercept-one [Virasoro constraints](../../../../../virasoro-constraint.md), with noncompact $k^2=-M^2$, give

$$
M^2=\sum_j(p_L^j)^2+\frac4{\alpha'}(\widetilde N-1)
=\sum_j(p_R^j)^2+\frac4{\alpha'}(N-1).
$$

Thus the mass formula and [compact-circle closed-string level matching](../../../../../compact-circle-closed-string-level-matching.md) condition are

$$
\boxed{M^2=\sum_j\left[\frac{n_j^2}{R_j^2}+\frac{w_j^2R_j^2}{\alpha'^2}\right]+\frac2{\alpha'}(N+\widetilde N-2),\qquad
\widetilde N-N+\sum_j n_jw_j=0.}
$$

Here $N$ labels right movers and $\widetilde N$ left movers; exchanging the labels changes the displayed sign convention, not the spectrum. Noncompact oscillator polarizations are still restricted by positive-mode Virasoro conditions and null-state identifications. [T-duality](../../../../../t-duality.md) exchanges $n_j,w_j$ and $R_j,\alpha'/R_j$, preserving masses and the physical state conditions.

At generic radius, neutral $(N,\widetilde N)=(1,1)$ states with one noncompact oscillator and one compact oscillator give two massless vectors per circle. They are the two Abelian gauge fields associated with the compact metric and two-form components. Additional charged vectors can occur at oscillator level sum one. For one circle, set all other compact charges to zero. Take $n=w=\pm1$ and $(N,\widetilde N)=(1,0)$, with a right-moving noncompact oscillator $\alpha_{-1}^\mu$; or take $n=-w=\pm1$ and $(N,\widetilde N)=(0,1)$, with a left-moving noncompact oscillator $\widetilde\alpha_{-1}^\mu$. These obey level matching. Their common squared mass is

$$
M_{
m extra}^2=\frac1{R^2}+\frac{R^2}{\alpha'^2}-\frac2{\alpha'}
=\left(\frac R{\alpha'}-\frac1R\right)^2.
$$

Therefore **four extra charged vector particles become massless at $R=\sqrt{\alpha'}$**, the [self-dual circle](../../../../../self-dual-circle-compactification.md). Away from that radius they are massive. They are genuine vector states: the noncompact level-one oscillator carries a vector polarization, and the Virasoro constraint plus its null identification impose transversality and remove the gauge polarization at zero mass.

The resulting [self-dual circle current algebra](../../../../../self-dual-circle-current-algebra.md) makes the gauge enhancement explicit. At the special radius, the left-moving charges above have $p_L=\pm2/\sqrt{\alpha'}$, $p_R=0$. With $Y_L(z)Y_L(w)\sim-\alpha'\log(z-w)/2$, the currents

$$
J_L^3=\frac{i\partial Y_L}{\sqrt{\alpha'}},\qquad J_L^\pm=:e^{\pm2iY_L/\sqrt{\alpha'}}:
$$

have conformal weight one. The operator products give $J^3J^3\sim1/[2(z-w)^2]$, $J^3J^\pm\sim\pm J^\pm/(z-w)$ and $J^+J^-\sim1/(z-w)^2+2J^3/(z-w)$. They form a level-one SU(2) current algebra; the right-moving copy supplies another SU(2). Pairing each chiral current with the opposite-sector noncompact derivative yields a weight-$(1,1)$ vector vertex. Thus the generic $U(1)_L\times U(1)_R$ becomes **$SU(2)_L\times SU(2)_R$**, with four charged generators in addition to the two Cartan vectors. Several self-dual circles give the corresponding product enhancement.

Compactification also creates scalar states and moduli; not every additional massless state is a vector. The mechanism just shown uses the intercept-one bosonic spectrum. A superstring projection changes the allowed oscillator states, so the same mass formula cannot simply be applied to a GSO-projected superstring without modification.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
