<h1 id="section-b/12/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Shockley-Queisser limit](../../../../../../shockley-queisser-limit.md) is a radiative detailed-balance limit for a single-junction photovoltaic device under specified illumination and temperature. Its idealized absorber collects above-gap photons, thermalizes their excess energy and loses carriers only through the radiative processes required by absorptance and emission. Sub-gap photons are not harvested. A favorable gap balances current loss at large gap against voltage loss at small gap.[Journal of Applied Physics 32 (1961), pp. 510–519; radiative detailed balance and illumination assumptions](../../../../../../detailed-balance-limit-of-efficiency-of-p-n-junction-solar-cells-by-william-shockley-and-hans-j-queisser.md)

For a step-like absorber,

$$
J_{\rm SC}=q\int_{E_g}^{\infty}\Phi_{\rm sun}(E)\,dE,
\qquad
\boxed{V_{\rm OC}^{\rm rad}=\frac{k_BT_c}{q}
\ln\left(1+\frac{J_{\rm SC}}{J_0^{\rm rad}}\right)}.
$$

The dark radiative current decreases rapidly with gap, so the qualitative ordering for the supplied absorbers is

$$
\boxed{V_{\rm OC}^{\rm rad}(\mathrm{CsSnI_3})
<V_{\rm OC}^{\rm rad}(\mathrm{CsPbI_3})
<V_{\rm OC}^{\rm rad}(\mathrm{CsPbBr_3})}.
$$

The curve rises beneath the diagonal $V=E_g/q$. The deficit $\Delta V=E_g/q-V_{\rm OC}^{\rm rad}$ reflects finite-temperature carrier statistics and the entropy associated with absorption and emission, including angular dilution of sunlight. Under ordinary unconcentrated illumination it is of order a few tenths of a volt, with a weaker gap dependence than $V_{\rm OC}$ itself. In a fixed blackbody-sun model its absolute value grows modestly with increasing gap, while its fraction of $E_g/q$ decreases. Above-gap thermalization is an efficiency loss but is not, by itself, the definition of this voltage deficit.

<a id="section-b/12/ii/image-an-explicit-radiative-model-illustrates-the-band-gap-and-voltage-deficit-trends"></a>
![](../../../../../../past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2023/paper-1-additional-solar-limit.png)

**[Figure 9](#section-b/12/ii/image-an-explicit-radiative-model-illustrates-the-band-gap-and-voltage-deficit-trends). An explicit radiative model illustrates the band-gap and voltage-deficit trends**. Original detailed-balance calculation for a 6000 K blackbody sun, a 300 K cell, a solar angular radius of 0.00465 radians, a step absorber and emission into one hemisphere. The three plotted gaps are supplied values; the resulting voltages illustrate these declared assumptions, not measured device voltages or an unspecified AM1.5G calculation.

A measured perovskite device can have a larger deficit from nonradiative recombination and contact losses. The gaps alone do not determine those material-specific losses or a unique numerical voltage: solar spectrum, concentration, cell temperature and optical emission geometry must also be specified.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12](../../12.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
