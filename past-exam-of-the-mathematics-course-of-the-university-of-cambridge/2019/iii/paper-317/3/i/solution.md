<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume zero temperature, complete ionization, constant composition, noninteracting electrons, negligible ion thermal pressure, and Newtonian stellar gravity. Ions supply almost all the mass, while [electron degeneracy pressure](../../../../../../electron-degeneracy-pressure.md) supplies support. By the [Pauli exclusion principle](../../../../../../pauli-exclusion-principle.md), the two electron spin states fill a momentum sphere up to [Fermi momentum](../../../../../../fermi-momentum.md) $p_F$. Counting states gives

$$
n_e=\frac{2}{(2\pi\hbar)^3}\frac{4\pi p_F^3}{3}
=\frac{p_F^3}{3\pi^2\hbar^3},\qquad
\rho=\mu_em_un_e,
$$

where $\mu_e$ is [mean molecular weight per electron](../../../../../../mean-molecular-weight-per-electron.md). The momentum flux of this isotropic [Fermi gas](../../../../../../fermi-gas.md) is

$$
P=\frac{2}{3(2\pi\hbar)^3}\int_{p\le p_F}p\,v(p)\,d^3p
=\frac1{3\pi^2\hbar^3}\int_0^{p_F}\frac{p^4c^2}{\sqrt{m_e^2c^4+p^2c^2}}\,dp.
$$

Writing $x=p_F/(m_ec)$ and performing the integral gives the [equation of state of a cold electron gas](../../../../../../equation-of-state-of-a-cold-electron-gas.md)

$$
\boxed{P=\frac{m_e^4c^5}{24\pi^2\hbar^3}
\left[x(2x^2-3)\sqrt{1+x^2}+3\operatorname{arsinh}x\right],\qquad
x=\frac{\hbar}{m_ec}\left(\frac{3\pi^2\rho}{\mu_em_u}\right)^{1/3}.}
$$

In the nonrelativistic limit $p_F\ll m_ec$, $v(p)\simeq p/m_e$, so

$$
\boxed{P=K_{\rm NR}\rho^{5/3},\qquad
K_{\rm NR}=\frac{\hbar^2(3\pi^2)^{2/3}}{5m_e(\mu_em_u)^{5/3}}.}
$$

In the ultrarelativistic limit $p_F\gg m_ec$, $v(p)\simeq c$, so

$$
\boxed{P=K_{\rm R}\rho^{4/3},\qquad
K_{\rm R}=\frac{\hbar c(3\pi^2)^{1/3}}{4(\mu_em_u)^{4/3}}.}
$$

These are [polytropic equations of state](../../../../../../polytropic-equation-of-state.md) with indices $3/2$ and $3$, respectively. The relativistic softening underlies the [Chandrasekhar mass](../../../../../../chandrasekhar-limit.md) limit; Coulomb corrections, thermal effects, rotation, and general relativity are excluded from this idealized derivation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
