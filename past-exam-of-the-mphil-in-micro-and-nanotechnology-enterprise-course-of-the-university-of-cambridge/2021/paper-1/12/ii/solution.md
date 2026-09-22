<h1 id="12/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The illuminated area and incident [power](../../../../../power.md) are

$$
A=(0.04)^2=1.6\times10^{-3}\,\mathrm{m^2},\qquad
P_{\rm in}=87A=0.1392\,\mathrm W.
$$

A $412\,\mathrm{nm}$ [photon](../../../../../photon.md) has [energy](../../../../../energy-split.md) $hc/\lambda=4.821\times10^{-19}\,\mathrm J=3.01\,\mathrm{eV}$, above the [silicon](../../../../../silicon.md) [band gap](../../../../../band-gap.md). With one collected [electron](../../../../../electron.md) per [photon](../../../../../photon.md),

$$
I_{\rm ph}=q\frac{P_{\rm in}\lambda}{hc}=0.0462562\,\mathrm A.
$$

Use the ideal-diode approximation with **ideality factor $n=1$**, negligible shunt leakage and the same dark [diode](../../../../../diode.md) parameters under illumination. At $300\,\mathrm K$, $V_T=k_BT/q=0.025852\,\mathrm V$. The measured dark point then fixes

$$
I_0=\frac{10^{-4}}{\exp(0.466/V_T)-1}=1.4844\times10^{-12}\,\mathrm A.
$$

At open circuit the forward [diode](../../../../../diode.md) [electric current](../../../../../electric-current.md) balances the photocurrent:

$$
\boxed{V_{\rm oc}=V_T\ln\!\left(1+\frac{I_{\rm ph}}{I_0}\right)=0.62465\,\mathrm V\simeq0.625\,\mathrm V}.
$$

This is below the $1.1\,\mathrm{eV}$ [band gap](../../../../../band-gap.md) expressed per elementary charge. Excess [photon](../../../../../photon.md) [energy](../../../../../energy-split.md) does not translate directly into terminal [voltage](../../../../../voltage.md); much of it thermalizes.

The paper does not explicitly specify an ideality factor. If it is not taken as unity, one dark operating point cannot determine both $I_0$ and $n$. The corresponding family is

$$
V_{\rm oc}(n)=nV_T\ln\!\left[1+\frac{I_{\rm ph}}{10^{-4}}\left(\exp\!\left(\frac{0.466}{nV_T}\right)-1\right)\right].
$$

Thus $0.625\,\mathrm V$ is a stated-model estimate, not a parameter-free inference from that one measurement.

## ↑ Ancestors (10)

1. [Ii](../ii.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../split.md)
6. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
