<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

In the nonrelativistic dilute regime, $E(p)=mc^2+p^2/(2m)+\cdots$ and the [Fermi-Dirac distribution](../../../../../fermi-dirac-distribution.md) reduces to the [Maxwell-Boltzmann distribution](../../../../../maxwell-boltzmann-distribution.md). Hence

$$
n\simeq\frac{4\pi}{h^3}e^{(\mu-mc^2)/(kT)}
\int_0^\infty p^2e^{-p^2/(2mkT)}dp.
$$

Differentiating the [Gaussian integral](../../../../../gaussian-integral.md) with respect to its coefficient gives $\int_0^\infty p^2e^{-ap^2}dp=\sqrt\pi/(4a^{3/2})$. Therefore

$$
\boxed{n\simeq\left(\frac{2\pi mkT}{h^2}\right)^{3/2}e^{(\mu-mc^2)/(kT)}}.
$$

The degeneracy factor here is the one in the supplied integral, namely one. Substituting $kT=mc^2/\alpha$, $\mu=0$ and dividing by the supplied [photon](../../../../../photon.md) density gives

$$
\boxed{\frac n{n_\gamma}=\frac{\sqrt{2\pi}}{8\zeta(3)}\alpha^{3/2}e^{-\alpha}}.
$$

At $\alpha=20$ this is about $4.8\times10^{-8}$. The relic is already nonrelativistic at decoupling and becomes still colder as its momenta redshift, making it a possible [cold dark matter](../../../../../cold-dark-matter.md) component if it is stable and interacts sufficiently weakly with light.

For orientation, write $\eta_b=n_b/n_\gamma$. Ignoring subsequent [entropy](../../../../../entropy.md) transfer, its density relative to baryons would be $\rho_X/\rho_b=(1/20)(n/n_\gamma)/\eta_b$. With the cosmological baryon-to-photon ratio of order $6\times10^{-10}$, this is of order four, demonstrating the right cosmological scale. The measured dark-to-baryonic density ratio is likewise of order five; an observational reference is [https://arxiv.org/abs/1807.06209](https://arxiv.org/abs/1807.06209) . This is a candidate abundance argument, not an exact relic-density calculation: [photon](../../../../../photon.md) heating after decoupling changes $n/n_\gamma$, and stability and interaction properties were not specified. The supplied mass and freeze-out parameter alone therefore do not establish a precise fit.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
