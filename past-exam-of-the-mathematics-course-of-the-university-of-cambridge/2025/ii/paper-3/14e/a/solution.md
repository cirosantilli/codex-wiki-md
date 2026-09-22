<h1 id="14e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The Bose--Einstein and Fermi--Dirac occupation factors are

$$
\frac1{\exp((E-\mu)/(k_BT))\mp1}.
$$

In the stated nonrelativistic dilute regime, $E-\mu$ is dominated by $mc^2$, so the exponential is large and either denominator is asymptotic to $\exp((E-\mu)/(k_BT))$. Integrating the resulting Maxwell--Boltzmann occupation over momentum states gives

$$
n=\frac{4\pi g_s}{h^3}\int_0^\infty
p^2e^{-[E(p)-\mu]/(k_BT)}\,dp.
$$

For $E=mc^2+p^2/(2m)$, integration by parts or differentiation of the supplied Gaussian integral gives

$$
\int_0^\infty p^2e^{-p^2/(2mk_BT)}\,dp
=\frac{\sqrt\pi}{4}(2mk_BT)^{3/2}.
$$

Consequently

$$
\boxed{
n=g_s\left(\frac{2\pi mk_BT}{h^2}\right)^{3/2}
e^{(\mu-mc^2)/(k_BT)}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14E](../../14e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
