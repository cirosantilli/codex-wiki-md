<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $\hbar=c=k_B=1$ and count one populated helicity per [neutrino](../../../../../../neutrino.md) or [antineutrino](../../../../../../antineutrino.md). For massless particles, the [Fermi-Dirac distribution](../../../../../../fermi-dirac-distribution.md) gives

$$
\rho_\nu=\frac1{2\pi^2}\int_0^\infty dp\,
\frac{p^3}{e^{(p-\mu_\nu)/T_\nu}+1}.
$$

When $\mu_\nu/T_\nu\gg1$, the occupied states form an almost sharp [Fermi sea](../../../../../../fermi-sea.md). Replacing the distribution by $\Theta(\mu_\nu-p)$ gives

$$
\boxed{\rho_\nu\simeq\frac1{2\pi^2}\int_0^{\mu_\nu}p^3\,dp
=\frac{\mu_\nu^4}{8\pi^2}}.
$$

The relative finite-temperature correction is of order $(T_\nu/\mu_\nu)^2$.

Chemical equilibrium gives $\mu_{\bar\nu}=-\mu_\nu$. For positive large $\mu_\nu$, the corresponding [antineutrino](../../../../../../antineutrino.md) distribution is dilute, so

$$
\rho_{\bar\nu}\simeq\frac{e^{-\mu_\nu/T_\nu}}{2\pi^2}\int_0^\infty p^3e^{-p/T_\nu}dp
=\frac{3T_\nu^4}{\pi^2}e^{-\mu_\nu/T_\nu}.
$$

It is exponentially negligible. The [neutrino degeneracy parameter](../../../../../../neutrino-degeneracy-parameter.md) $\xi_\nu=\mu_\nu/T_\nu$ is conserved in the assumed adiabatic massless evolution: redshifting preserves the distribution with both $T_\nu$ and $\mu_\nu$ proportional to $a^{-1}$.

There is a sign qualification in the printed absolute-value formula. If $\mu_\nu<0$, the distribution of [neutrinos](../../../../../../neutrino.md) themselves is exponentially suppressed, and the [antineutrinos](../../../../../../antineutrino.md), with positive [chemical potential](../../../../../../chemical-potential.md), form the degenerate sea. In either case the [degenerate neutrino and antineutrino energy density](../../../../../../degenerate-neutrino-and-antineutrino-energy-density.md) is

$$
\boxed{\rho_\nu+\rho_{\bar\nu}\simeq\frac{|\mu_\nu|^4}{8\pi^2}}.
$$

Thus the formula with $|\mu_\nu|$ describes the dominant member of the pair, or their leading total, rather than the named [neutrino](../../../../../../neutrino.md) distribution for both signs. No extra factor of two is present: only one member is densely occupied. Additional populated internal states multiply the result by their degeneracy.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
