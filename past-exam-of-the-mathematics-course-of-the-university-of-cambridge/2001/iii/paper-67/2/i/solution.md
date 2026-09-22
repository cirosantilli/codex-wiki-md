<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [natural units](../../../../../../natural-units.md) with $c=\hbar=k_B=1$ and the unreduced [Planck mass](../../../../../../planck-mass.md) $M_{\rm Pl}=G^{-1/2}$. In a [radiation-dominated universe](../../../../../../radiation-dominated-universe.md), the [effective number of relativistic energy degrees of freedom](../../../../../../effective-number-of-relativistic-energy-degrees-of-freedom.md) $g_*=\mathcal N$ gives

$$
\rho_r=\frac{\pi^2}{30}g_*T^4,\qquad
H^2=\frac{8\pi G}{3}\rho_r,\qquad
H=\sqrt{\frac{8\pi^3}{90}}\frac{\sqrt{g_*}T^2}{M_{\rm Pl}}
\simeq1.66\frac{\sqrt{g_*}T^2}{M_{\rm Pl}}.
$$

The ratio of weak conversion rate to expansion rate is proportional to $T^3$, so it decreases as the universe cools. [Cosmological weak freeze-out](../../../../../../cosmological-weak-freeze-out.md) occurs approximately at $\Gamma=H$, giving

$$
\boxed{T_d\simeq
\left(\frac{1.66\sqrt{g_*}}{G_F^2M_{\rm Pl}}\right)^{1/3}
\sim1\text{--}2\ {\rm MeV}.}
$$

For $g_*=10.75$, $G_F=10^{-5}\ {\rm GeV}^{-2}$ and $M_{\rm Pl}=1.22\times10^{19}\ {\rm GeV}$ this estimate is $1.65\ {\rm MeV}$. Equivalently $g_*^{1/6}\simeq1.5$ is only a mild multiplicative correction. The rate itself was given only to order of magnitude, so this is a decoupling scale, not a precise prediction for the weak freeze-out abundance.

Both [neutrons](../../../../../../neutron.md) and [protons](../../../../../../proton.md) are nonrelativistic at this [temperature](../../../../../../temperature.md). The [nonrelativistic Maxwell--Boltzmann number density](../../../../../../nonrelativistic-maxwell-boltzmann-number-density.md) follows by the Gaussian momentum integral:

$$
n_i=g_i\int\frac{d^3p}{(2\pi)^3}
e^{-(m_i+p^2/(2m_i)-\mu_i)/T}
=g_i\left(\frac{m_iT}{2\pi}\right)^{3/2}e^{(\mu_i-m_i)/T}.
$$

Their equal spin degeneracies are $g_n=g_p=2$. [Chemical equilibrium](../../../../../../chemical-equilibrium.md) of the weak reaction gives $\mu_n+\mu_{\nu_e}=\mu_p+\mu_e$; with negligible lepton asymmetry, $\mu_n\simeq\mu_p$. Taking the ratio and setting the nearly equal nucleon masses equal only in the prefactor gives the [neutron-proton chemical equilibrium](../../../../../../neutron-proton-chemical-equilibrium.md) result

$$
\frac{n_n}{n_p}
=\left(\frac{m_n}{m_p}\right)^{3/2}
e^{(\mu_n-\mu_p-Q)/T}
\simeq e^{-Q/T},\qquad
\boxed{\frac{X_n}{X_p}\simeq e^{-Q/T_d}.}
$$

The common baryon normalization cancels. Keeping the exact mass prefactor changes this by only order $Q/m_p$. Thus the printed simple exponential is the usual nonrelativistic equal-mass-prefactor approximation. Using $Q\simeq1.29\ {\rm MeV}$ with the rough decoupling scale above gives a ratio of order one half; the rate's omitted numerical factors and gradual freeze-out must be included before using a more accurate neutron abundance.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
