<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the standard local [chemical quench level](../../../../../../chemical-quench-level.md) approximation: [carbon monoxide](../../../../../../carbon-monoxide.md)-rich gas from the hot deep region is transported upward, and conversion becomes slower as the gas enters the cooler layers. Assume that neither a faster loss process nor strong compositional fractionation removes [carbon monoxide](../../../../../../carbon-monoxide.md) above the quench level. For an effective mixing length $L$, the [eddy mixing time](../../../../../../eddy-mixing-time.md) is $\tau_{\rm mix}\simeq L^2/K_{zz}$, so outrunning conversion near $1\,\mathrm{bar}$ requires

$$
\boxed{K_{zz}\gtrsim\frac{L^2}{10^5\,\mathrm{s}}}.
$$

The usual order-of-magnitude choice is $L\simeq h_b$, the local [atmospheric scale height](../../../../../../atmospheric-scale-height.md) at $T_b=1400\,\mathrm{K}$. Equal planetary mass and radius give the same gravity as [Jupiter](../../../../../../jupiter.md); with the same [mean molecular weight](../../../../../../mean-molecular-weight.md), the [atmospheric scale height](../../../../../../atmospheric-scale-height.md) scales linearly with [temperature](../../../../../../temperature.md). To use the supplied $30\,\mathrm{km}$ reference, additionally adopt a representative Jovian reference [temperature](../../../../../../temperature.md) $T_J=150\,\mathrm{K}$. Then

$$
h_b\simeq30\,\mathrm{km}\frac{1400}{150}\simeq280\,\mathrm{km},\qquad
\boxed{K_{zz}\gtrsim8\times10^5\,\mathrm{m^2\,s^{-1}}\simeq8\times10^9\,\mathrm{cm^2\,s^{-1}}}.
$$

Using $k_BT/(\mu m_Hg)$ directly with $\mu\simeq2.3$ and Jovian $g\simeq25\,\mathrm{m\,s^{-2}}$ gives $h_b\simeq200\,\mathrm{km}$ and $K_{zz}\gtrsim4\times10^5\,\mathrm{m^2\,s^{-1}}$, the same order of magnitude. The supplied Jovian height is approximate and does not specify its reference [temperature](../../../../../../temperature.md). Inserting $30\,\mathrm{km}$ unchanged for the hot gas would instead give $9\times10^3\,\mathrm{m^2\,s^{-1}}$ and neglect this temperature scaling.

The pressure separation is relevant to a stronger, whole-column transport estimate. With constant gravity and [mean molecular weight](../../../../../../mean-molecular-weight.md), the profile gives

$$
\begin{aligned}
\Delta z&=\int_{10^{-3}\,\rm bar}^{1\,\rm bar}h(P)\,d\ln P\\
&=\frac{30\,\mathrm{km}}{150\,\mathrm{K}}\left[\frac{1400+500}{2}\ln100+500\ln10\right]\simeq1.1\times10^3\,\mathrm{km}.
\end{aligned}
$$

If one additionally requires diffusion through the entire column within $10^5\,\mathrm{s}$, a sufficient conservative condition is $K_{zz}\gtrsim\Delta z^2/\tau_{\rm chem}\sim10^7\,\mathrm{m^2\,s^{-1}}$. It is not a necessary local quench condition: the [chemical relaxation time](../../../../../../chemical-relaxation-time.md) is expected to become much longer in the cooler gas, so a longer total transit time can still preserve [carbon monoxide](../../../../../../carbon-monoxide.md).

**The usual quench estimate is $K_{zz}$ of order $10^6\,\mathrm{m^2\,s^{-1}}$ under the stated scale-height assumptions.** A unique bound for survival to $10^{-3}\,\mathrm{bar}$ cannot be inferred from one reaction time without assumptions about its variation, the mixing length and upper-atmospheric losses.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
