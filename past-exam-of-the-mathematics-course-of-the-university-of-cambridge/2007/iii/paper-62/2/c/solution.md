<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $n_b=n_p+n_H$ for the [cosmological baryon density](../../../../../../cosmological-baryon-density.md) in this hydrogen-only model, and $x_e=n_p/n_b$ for the [hydrogen ionization fraction](../../../../../../hydrogen-ionization-fraction.md). By [charge neutrality](../../../../../../charge-neutrality.md), $n_e=n_p$, so the [Saha ionization equation](../../../../../../saha-ionization-equation.md) becomes

$$
\frac{1-x_e}{x_e^2}=n_b\left(\frac{2\pi}{M_eT}\right)^{3/2}e^{B/T}.
$$

The [baryon-to-photon ratio](../../../../../../baryon-to-photon-ratio.md) is $\eta=n_b/n_\gamma$, and the equilibrium [photon number density](../../../../../../photon-number-density.md) is $n_\gamma=2\zeta(3)T^3/\pi^2$. At an order-one [hydrogen ionization fraction](../../../../../../hydrogen-ionization-fraction.md), neglecting factors of order one therefore gives

$$
1\simeq\eta\left(\frac T{M_e}\right)^{3/2}e^{B/T},\qquad T\simeq\frac{B}{\log[\eta^{-1}(M_e/T)^{3/2}]}.
$$

Replacing $T$ inside the slowly varying logarithm by $B$ gives

$$
\boxed{T\simeq\frac{B}{\log[\eta^{-1}(M_e/B)^{3/2}]}\ll B.}
$$

With $B=13.6\,\mathrm{eV}$, $M_e=5\times10^5\,\mathrm{eV}$ and $\eta=10^{-10}$, this is $T\simeq0.351\,\mathrm{eV}\simeq4.1\times10^3\,\mathrm K$. Solving the preceding implicit approximation instead gives $T\simeq0.306\,\mathrm{eV}\simeq3.5\times10^3\,\mathrm K$. Both are reasonable estimates of the [recombination temperature](../../../../../../recombination-temperature.md) at the accuracy requested. The [small baryon abundance delays hydrogen recombination](../../../../../../small-baryon-abundance-delays-hydrogen-recombination.md): even when $T\ll B$, the high-energy tail of the abundant [photons](../../../../../../photon.md) can still ionize the much rarer [hydrogen atoms](../../../../../../hydrogen-atom.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
