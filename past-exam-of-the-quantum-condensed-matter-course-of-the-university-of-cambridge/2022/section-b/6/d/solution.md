<h1 id="section-b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An ideal diffusion-dominated [p-n junction](../../../../../p-n-junction.md) obeys the [Shockley diode equation](../../../../../shockley-diode-equation.md)

$$
\boxed{I(V,T)=I_s(T)\left[e^{eV/(\eta k_BT)}-1\right],}
$$

with [diode ideality factor](../../../../../diode-ideality-factor.md) $\eta=1$ in the simplest model. Forward bias gives exponential current growth; reverse bias gives a nearly constant $-I_s$ until [diode reverse breakdown](../../../../../diode-reverse-breakdown.md), outside this ideal expression.

For a long abrupt [p-n junction](../../../../../p-n-junction.md) in low [carrier injection](../../../../../carrier-injection.md), the [diode saturation current](../../../../../diode-saturation-current.md) is

$$
\boxed{I_s=e\mathcal A n_i^2\left(\frac{D_p}{L_pN_D}+\frac{D_n}{L_nN_A}\right)=C(T)n_i^2.}
$$

Here $\mathcal A$ is area, $N_D,N_A$ are ionized dopant densities, and $D,L$ are minority-carrier diffusion coefficients and diffusion lengths in the appropriate regions. At each temperature, extract $I_s$ either from the reverse-saturation plateau below breakdown or from a forward exponential fit using its measured [diode ideality factor](../../../../../diode-ideality-factor.md).

[Extracting a semiconductor band gap from diode saturation current](../../../../../extracting-a-semiconductor-band-gap-from-diode-saturation-current.md) requires correcting for the transport prefactor:

$$
\boxed{\log\frac{I_s(T)}{C(T)T^3}=\text{constant}-\frac{E_g}{k_BT}.}
$$

A plot against $1/T$ has slope $-E_g/k_B$ when the gap and effective masses are nearly temperature-independent. Alternatively divide the measured $I_s$ by a known $C(T)$ to recover the full $n_i^2(T)$. The prefactor cannot generally be assumed constant over an arbitrarily broad range. Junction-generation or recombination-dominated current can scale as $n_i$ instead, so the diffusion regime should be identified from the current-voltage behaviour.

<a id="section-b/6/d/image-ideal-diode-characteristic-and-extraction-of-a-semiconductor-activation-energy"></a>
![](../../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2022-q6-junction-and-activation.png)

**[Figure 3](#section-b/6/d/image-ideal-diode-characteristic-and-extraction-of-a-semiconductor-activation-energy). Ideal diode characteristic and extraction of a semiconductor activation energy**. Original model sketches. The normalized current-voltage curve shows forward exponential growth and reverse saturation. The activation panel plots a model proportional to $n_i^2/T^3$ for a fixed illustrative gap; it shows the slope to infer after correcting transport prefactors, not measured device data.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter course of the University of Cambridge](../../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
