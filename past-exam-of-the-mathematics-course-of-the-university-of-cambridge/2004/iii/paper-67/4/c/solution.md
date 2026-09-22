<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [absorption distance](../../../../../../absorption-distance.md) $X$ and its distribution $f_X$. Summing hydrogen columns per unit $X$ gives $\int N f_X\,dN$. The physical light-path length per $X$ is

$$
\frac{d\ell}{dX}=\frac{c}{H_0(1+z)^3}.
$$

The mean neutral-hydrogen [number density](../../../../../../number-density.md) is therefore $(H_0/c)(1+z)^3\int N f_X\,dN$. Divide by $(1+z)^3$ to obtain its comoving [density](../../../../../../density.md), multiply by hydrogen atomic mass, and divide by today's mass [critical density](../../../../../../critical-density.md) $\rho_{\rm crit,0}=3H_0^2/(8\pi G)$. This derives the [neutral gas density from an absorption distribution](../../../../../../neutral-gas-density-from-an-absorption-distribution.md):

$$
\boxed{\Omega_{\rm HI}(z)=\frac{H_0m_H}{c\rho_{\rm crit,0}}\int N f_X(N,z)\,dN.}
$$

If “neutral gas” includes [helium](../../../../../../helium.md), replace $m_H$ by $\mu_Hm_H$, with a stated abundance correction approximately $\mu_H\simeq1.3$. Equivalently, for the distribution per redshift the prefactor inside the integral is $m_H H(z)/[c\rho_{\rm crit,0}(1+z)^2]$ multiplying $Nf_z$. In the PDF's energy-density convention, both the mass [density](../../../../../../density.md) and [critical density](../../../../../../critical-density.md) are multiplied by $c^2$, leaving their ratio unchanged. The usual quoted abundance uses comoving mass [density](../../../../../../density.md) relative to today's [critical density](../../../../../../critical-density.md); a ratio of physical [density](../../../../../../density.md) to the epoch's [critical density](../../../../../../critical-density.md) instead multiplies this answer by $(1+z)^3H_0^2/H(z)^2$.

To infer total gas, one needs the neutral fraction $x_{\rm HI}=N_{\rm HI}/N_H$ for each absorber. The [ionized gas density from an absorption distribution](../../../../../../ionized-gas-density-from-an-absorption-distribution.md) is

$$
\boxed{\Omega_g(z)=\frac{H_0\mu_Hm_H}{c\rho_{\rm crit,0}}
\int\frac{N}{x_{\rm HI}(N,z)}f_X(N,z)\,dN.}
$$

This is an ionization-corrected integral, not an inference available from the observed columns alone. For optically thin, almost fully ionized hydrogen, [photoionization equilibrium](../../../../../../photoionization-equilibrium.md) gives $\Gamma n_{\rm HI}=\alpha(T)n_en_{\rm HII}\simeq\alpha(T)n_H^2$. If the absorbing depth $L$ is specified, $N=\alpha(T)n_H^2L/\Gamma$ and

$$
N_H=n_HL=\left(\frac{\Gamma NL}{\alpha(T)}\right)^{1/2}.
$$

Thus [photoionization rate](../../../../../../photoionization-rate.md), [temperature](../../../../../../temperature.md) and depth are all needed.

One useful physical closure sets $L$ to a local [Jeans length](../../../../../../jeans-length.md), $L\propto(f_gT/n_H)^{1/2}$, with local gas fraction $f_g$. Solving $N\propto[\alpha(T)/\Gamma](f_gT)^{1/2}n_H^{3/2}$ then gives the [Jeans-length ionization correction for the Lyman-alpha forest](../../../../../../jeans-length-ionization-correction-for-the-lyman-alpha-forest.md):

$$
N_H\propto N^{1/3}\Gamma^{1/3}\left(\frac{f_gT}{\alpha(T)}\right)^{1/3},\qquad
\Omega_g\propto\Gamma^{1/3}\left(\frac{f_gT}{\alpha(T)}\right)^{1/3}\int N^{1/3}f_X\,dN.
$$

This illustrates why weak, highly ionized forest lines can dominate the total gas inventory even though [damped Lyman-alpha systems](../../../../../../damped-lyman-alpha-system.md) dominate the neutral-column-weighted inventory. It is a model for locally confined optically thin gas; optically thick [Lyman limit systems](../../../../../../lyman-limit-system.md) and [damped Lyman-alpha systems](../../../../../../damped-lyman-alpha-system.md) require a separate [radiative transfer](../../../../../../radiative-transfer.md) treatment. The physical basis and observational application of this closure are developed in [Schaye's absorption-based matter-density calculation](https://arxiv.org/abs/astro-ph/0104272).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
