<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the dark-sector [temperature](../../../../../../temperature.md) in every dimensionless integration variable: $x=m_\phi/T_\phi$ and $y=p/T_\phi$. Assume a single real [scalar field](../../../../../../scalar-field.md), $g=1$, and fast number-changing reactions keeping $\mu_\phi=0$. For $x\gg1$, the populated momenta satisfy $y=O(\sqrt x)$, so

$$
\sqrt{x^2+y^2}=x+\frac{y^2}{2x}+O\left(\frac{y^4}{x^3}\right),\qquad
\frac1{e^{\sqrt{x^2+y^2}}-1}\simeq e^{-x-y^2/(2x)}.
$$

This is the nonrelativistic [Maxwell-Boltzmann distribution](../../../../../../maxwell-boltzmann-distribution.md) limit of the [Bose-Einstein distribution](../../../../../../bose-einstein-distribution.md). The given Gaussian [Gamma function](../../../../../../gamma-function.md) integral gives

$$
\int_0^\infty y^2e^{-y^2/(2x)}\,dy=\frac{\sqrt\pi}{4}(2x)^{3/2},\qquad
n\simeq\left(\frac{m_\phi T_\phi}{2\pi}\right)^{3/2}e^{-x}.
$$

Since $\rho_\phi=m_\phi n+3nT_\phi/2+\cdots$ and $P_\phi=nT_\phi$, the [entropy density at zero chemical potential](../../../../../../entropy-density-at-zero-chemical-potential.md) is $s_\phi=n(x+5/2+\cdots)$. Its leading [nonrelativistic entropy at zero chemical potential](../../../../../../nonrelativistic-entropy-at-zero-chemical-potential.md) is therefore

$$
\boxed{s_\phi\simeq\frac{m_\phi^3}{(2\pi)^{3/2}}x^{-1/2}e^{-x}.}
$$

An internal multiplicity $g$ would multiply this expression; the absence of $g$ in the printed result assumes a real one-state scalar.

Now use the constant [separately conserved visible and dark entropy](../../../../../../separately-conserved-visible-and-dark-entropy.md) ratio and the relativistic visible-bath entropy law, $s_{\rm SM}=(2\pi^2/45)g_{*s}^{\rm SM}T_\gamma^3=\xi s_\phi$. Since $T_\phi=m_\phi/x$,

$$
\left(\frac{T_\gamma}{T_\phi}\right)^3\simeq\frac{45}{2\pi^2(2\pi)^{3/2}}\frac\xi{g_{*s}^{\rm SM}}x^{5/2}e^{-x}.
$$

Thus the [cannibal-sector temperature ratio](../../../../../../cannibal-sector-temperature-ratio.md) has

$$
\boxed{\frac{T_\gamma}{T_\phi}\simeq k\left(\frac\xi{g_{*s}^{\rm SM}}\right)^{1/3}x^{5/6}e^{-x/3},\qquad k=\left[\frac{45}{2\pi^2(2\pi)^{3/2}}\right]^{1/3}.}
$$

The numerical coefficient is approximately $0.525$. The visible-bath temperature is the photon temperature while that bath is internally thermalized; after distinct visible species acquire different temperatures, its total entropy must instead use the appropriate temperature-weighted $g_{*s}^{\rm SM}$.

The displayed relativistic scalar entropy formula must not be continued into this regime with $g_{*s}^\phi=1$ held constant. If it is used as an effective definition at arbitrary temperature, then

$$
g_{*s}^{\phi}(x)\simeq\frac{45}{2\pi^2(2\pi)^{3/2}}x^{5/2}e^{-x},
$$

and $T_\gamma/T_\phi=(\xi g_{*s}^{\phi}/g_{*s}^{\rm SM})^{1/3}$ gives the same result. This specifies how the relativistic expression can legitimately be combined with the nonrelativistic one.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
