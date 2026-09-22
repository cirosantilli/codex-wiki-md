<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the reaction $p+e\leftrightarrow H+\gamma$, [chemical equilibrium](../../../../../../chemical-equilibrium.md) requires $\mu_p+\mu_e=\mu_H$ because thermal [photons](../../../../../../photon.md) have zero [chemical potential](../../../../../../chemical-potential.md). Insert the nonrelativistic [Maxwell-Boltzmann distribution](../../../../../../maxwell-boltzmann-distribution.md) number densities and use $m_H=m_p+m_e-\mathcal B$:

$$
\frac{n_en_p}{n_H}=\frac{g_eg_p}{g_H}\left(\frac{m_em_p}{m_H}\frac{T}{2\pi}\right)^{3/2}e^{-\mathcal B/T}.
$$

For ground-state [hydrogen](../../../../../../hydrogen.md), including its spin states, $g_e=g_p=2$, $g_H=4$; hence the degeneracy factor is one. Since $m_p/m_H\simeq1$, the right side is $(m_eT/2\pi)^{3/2}e^{-\mathcal B/T}$.

Charge neutrality gives $n_p=n_e$, while baryon conservation gives $n_b=n_p+n_H$. Consequently $n_e=n_p=X_en_b$ and $n_H=(1-X_e)n_b$. Inverting the preceding ratio and inserting the [photon number density](../../../../../../photon-number-density.md) with $n_b=\eta n_\gamma$ gives the [hydrogen-only Saha equation](../../../../../../hydrogen-only-saha-equation.md)

$$
\boxed{\frac{1-X_e}{X_e^2}=\frac{2\zeta(3)}{\pi^2}\eta\left(\frac{2\pi T}{m_e}\right)^{3/2}e^{\mathcal B/T}}.
$$

Writing $y=\mathcal B/T$, its coefficient is $(2\zeta(3)/\pi^2)\eta(2\pi\mathcal B/m_e)^{3/2}\simeq3.2\times10^{-16}$, consistent with the rounded $3\times10^{-16}$. The negligible mass-ratio correction and ground-state approximation are the assumptions behind this form.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
