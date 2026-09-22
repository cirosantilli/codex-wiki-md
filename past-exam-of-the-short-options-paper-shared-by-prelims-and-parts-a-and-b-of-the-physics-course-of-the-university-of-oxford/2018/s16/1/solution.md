<h1 id="s16/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume a dilute nondegenerate [hydrogen](../../../../hydrogen.md) [gas](../../../../gas.md) in thermal and [chemical equilibrium](../../../../chemical-equilibrium.md), with Maxwell-Boltzmann [translational partition functions](../../../../translational-partition-function.md), ground-state neutral [atoms](../../../../atom-physics.md), single [ionization](../../../../ionization.md) and [charge neutrality](../../../../charge-neutrality.md) $n_p=n_e$. For $\mathrm H\rightleftharpoons p+e$, [chemical equilibrium](../../../../chemical-equilibrium.md) gives $\mu_H=\mu_p+\mu_e$. The ideal-gas relation $\mu_i=E_{i0}+k_BT\log(n_i\lambda_i^3/g_i)$, with $E_{H0}=-R$, gives

$$
\frac{n_pn_e}{n_H}=\frac{g_pg_e}{g_H}\frac{\lambda_H^3}{\lambda_p^3\lambda_e^3}e^{-R/k_BT}.
$$

Neglecting the [electron](../../../../electron.md) [mass](../../../../mass.md) in $m_H/m_p$ and using the ground-state electronic statistical weights, $g_e=2$ and $g_H=2$ with cancelling nuclear-spin factors, this becomes

$$
\boxed{\frac{n_e^2}{n_H}=S(T)=\frac{(2\pi m_ek_BT)^{3/2}}{h^3}e^{-R/k_BT}.}
$$

Excited neutral states have an [energy](../../../../energy-split.md) gap of at least $3R/4$ above the ground state. At the [temperatures](../../../../temperature-split.md) relevant to the plotted maximum their [Boltzmann factors](../../../../boltzmann-factor.md) are very small despite the finite degeneracy increase. Highly excited levels also require a physical [plasma](../../../../plasma-physics.md) cutoff; the untruncated infinite isolated-atom partition sum is not a valid finite-density model. Ground-state dominance is an approximation in this regime, not a theorem at all [temperatures](../../../../temperature-split.md).

Take the heating process to keep the total hydrogen-nucleus [density](../../../../density.md) fixed, so $n_H+n_e=n_0$. This fixed-density assumption is needed to determine $n_0$ from the curve; freely expanding [gas](../../../../gas.md) would require its [density](../../../../density.md) history. The excited-to-ground ratio is $n_2/n_H\simeq4e^{-3R/(4k_BT)}$. Therefore

$$
\boxed{f=\frac{n_2}{n_0}\simeq4(1-x)e^{-3R/(4k_BT)}
=\frac4{1+n_e/n_H}e^{-3R/(4k_BT)},\qquad x=n_e/n_0.}
$$

At low [temperature](../../../../temperature-split.md) excitation is suppressed. At higher [temperature](../../../../temperature-split.md) excitation grows, but eventually [ionization](../../../../ionization.md) removes neutral [atoms](../../../../atom-physics.md) and the excited-neutral abundance decreases. To locate the maximum quantitatively, write $u=R/(k_BT)$. From $S/n_0=x^2/(1-x)$,

$$
\frac{dx}{d\log T}=\frac{x(1-x)}{2-x}\left(\frac32+u\right).
$$

Setting $d\log f/d\log T=0$ gives

$$
\boxed{x_{\max}=\frac{6u}{6+7u}.}
$$

Reading the original graph gives $T_{\max}\simeq(7.9\text{–}8.0)\times10^3$ K and $f_{\max}\simeq2.3\times10^{-7}$. With $R=13.6$ eV, this implies $u\simeq20$ and $\boxed{x_{\max}\simeq0.82}$. Substitution into

$$
\boxed{n_0=S(T_{\max})\frac{1-x_{\max}}{x_{\max}^2}}
$$

gives approximately $10^{18}\,\mathrm{m^{-3}}$. The result is particularly temperature-sensitive because of the Saha exponential; using $7900$ K gives about $9\times10^{17}\,\mathrm{m^{-3}}$, while the coarse $8000$ K reading gives about $1.2\times10^{18}\,\mathrm{m^{-3}}$. The plotted height is consistent with this range and should not be used to claim more precision than the source graph provides.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [S16](../../s16.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../split.md)
5. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
