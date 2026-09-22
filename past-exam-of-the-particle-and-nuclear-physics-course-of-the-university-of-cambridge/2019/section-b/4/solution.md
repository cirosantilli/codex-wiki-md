<h1 id="section-b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Dating principle**. Atmospheric [cosmic rays](../../../../cosmic-ray.md) produce secondary [neutrons](../../../../neutron-split.md), which can generate [carbon-14](../../../../carbon-14.md) through $^{14}\mathrm N(n,p){}^{14}\mathrm C$. [Carbon](../../../../carbon.md) then enters atmospheric [carbon dioxide](../../../../carbon-dioxide.md) and living organisms. While an organism exchanges carbon with its environment, its [carbon-14](../../../../carbon-14.md) to [carbon-12](../../../../carbon-12.md) ratio approximately tracks that reservoir. After exchange stops, surviving [carbon-14](../../../../carbon-14.md) undergoes [beta-minus decay](../../../../beta-minus-decay.md), whereas the stable [carbon](../../../../carbon.md) remains. On the closed-sample, constant-initial-ratio model, [radioactive decay](../../../../radioactive-decay.md) gives

$$
N_{14}(t)=N_{14}(0)e^{-\lambda t},\qquad
\mathcal A(t)=\lambda N_{14}(t)=\mathcal A_0e^{-\lambda t}.
$$

Thus [radiocarbon dating](../../../../radiocarbon-dating.md) infers elapsed time from the loss of an isotope ratio or of [radioactive activity](../../../../radioactive-activity.md) per fixed carbon mass. It dates cessation of carbon exchange, which need not equal the date an object was manufactured or buried. Actual calendar dating also requires [radiocarbon calibration](../../../../radiocarbon-calibration.md) and control of contamination and reservoir differences.

**Mean lifetime**. For [exponential decay](../../../../exponential-decay.md), the [half-life](../../../../half-life.md) obeys $e^{-\lambda T_{1/2}}=1/2$, while the [mean lifetime](../../../../mean-lifetime-physics.md) is $\tau=1/\lambda$. Hence

$$
\boxed{\tau=\frac{5730}{\ln2}\,\mathrm{yr}=8.26664\times10^3\,\mathrm{yr}.}
$$

Using $1\,\mathrm{yr}=365.25\times86400\,\mathrm s$ gives $\lambda=3.83325\times10^{-12}\,\mathrm s^{-1}$ and $\tau=2.60875\times10^{11}\,\mathrm s$.

**The mass minimum and beta stability**. Treat the supplied [masses](../../../../mass.md) as nuclear [rest energies](../../../../rest-energy.md) in $\mathrm{MeV}$, and omit [nuclear pairing](../../../../nuclear-pairing.md) as instructed. At fixed [mass number](../../../../mass-number.md) $A$, the volume and surface terms of the [semi-empirical mass formula](../../../../semi-empirical-mass-formula.md) are constant. Expanding the remaining terms gives a convex [nuclear mass parabola](../../../../nuclear-mass-parabola.md),

$$
M(A,Z)=C(A)+\left(\frac{a_C}{A^{1/3}}+\frac{4a_A}{A}\right)Z^2
+\left(m_p-m_n-4a_A\right)Z.
$$

The continuous minimum in [atomic number](../../../../atomic-number.md) is therefore

$$
\frac{\partial M}{\partial Z}
=m_p-m_n+\frac{2a_CZ}{A^{1/3}}-\frac{4a_A(A-2Z)}{A}=0,
\qquad
Z_* =\frac{4a_A+m_n-m_p}{2a_CA^{-1/3}+8a_A/A}.
$$

At $A=14$, the quadratic coefficient is $7.01302\,\mathrm{MeV}$ and $Z_*=6.79450$. The nearest integer is $Z=7$; the [nuclear isobar](../../../../isobar-nuclide.md) of minimum [mass](../../../../mass.md) is [nitrogen-14](../../../../nitrogen-14.md). Maximizing [nuclear binding energy](../../../../nuclear-binding-energy.md) alone would omit the neutron-proton rest-mass difference; its continuous optimum is slightly different, but also selects integer $Z=7$ here.

The values most useful for checking neighboring decay thresholds are

$$
\begin{array}{c|rrrr}
Z&5&6&7&8\\ \hline
M(14,Z)\;(\mathrm{MeV})&13065.584&13047.427&13043.296&13053.192.
\end{array}
$$

Consequently [carbon-14](../../../../carbon-14.md) can lower its nuclear [mass](../../../../mass.md) by changing a [neutron](../../../../neutron-split.md) into a [proton](../../../../proton.md):

$$
\boxed{{}^{14}_6\mathrm C\longrightarrow{}^{14}_7\mathrm N+e^-+\bar\nu_e
\quad\text{(beta-minus decay).}}
$$

For bare nuclear [masses](../../../../mass.md), the [Q value](../../../../q-value.md) must include the emitted [electron mass](../../../../electron-mass.md). Taking $m_ec^2=0.511\,\mathrm{MeV}$,

$$
Q_{\beta^-}^{\mathrm{model}}=M(14,6)-M(14,7)-m_ec^2
=4.13070-0.511=3.61970\,\mathrm{MeV}>0.
$$

The opposite proton-to-neutron conversion would lead to $Z=5$, whose nuclear [mass](../../../../mass.md) is $18.1567\,\mathrm{MeV}$ higher than that of [carbon-14](../../../../carbon-14.md). Neither [beta-plus decay](../../../../beta-plus-decay.md) nor [electron capture](../../../../electron-capture.md) can bridge that gap by supplying an electron-mass correction. For the [nitrogen-14](../../../../nitrogen-14.md) daughter, both neighboring nuclear [masses](../../../../mass.md) are higher: $Z=6$ by $4.13070\,\mathrm{MeV}$ and $Z=8$ by $9.89535\,\mathrm{MeV}$. Even [electron capture](../../../../electron-capture.md) to $Z=6$ has $Q=0.511-4.13070<0$. Thus the daughter has **no further energetically allowed single beta decay in this model**; physical [nitrogen-14](../../../../nitrogen-14.md) is stable.

These threshold numbers belong to the supplied smooth [semi-empirical mass formula](../../../../semi-empirical-mass-formula.md), not to an accurate prediction of the [carbon-14](../../../../carbon-14.md) electron spectrum or its long [half-life](../../../../half-life.md). [Semi-empirical mass errors can change beta-decay thresholds](../../../../semi-empirical-mass-errors-can-change-beta-decay-thresholds.md). Also, the instruction to omit [nuclear pairing](../../../../nuclear-pairing.md) is a model simplification: even $A=14$ does not make physical pairing vanish, and even-even carbon and odd-odd nitrogen need not have the same pairing correction. No omitted pairing coefficient is guessed here.

**Activity of modern carbon**. Neglect the small contribution of other stable [carbon](../../../../carbon.md) [isotopes](../../../../isotope.md) when counting atoms in a gram. The [Avogadro constant](../../../../avogadro-constant.md) gives

$$
N_{12}\simeq\frac{1\,\mathrm g}{12\,\mathrm{g\,mol^{-1}}}
(6.02214076\times10^{23}\,\mathrm{mol^{-1}})
=5.01845\times10^{22},
\qquad
N_{14}=1.3\times10^{-12}N_{12}=6.52399\times10^{10}.
$$

The expected [radioactive activity](../../../../radioactive-activity.md) of that one gram is

$$
\boxed{\mathcal A_0=\lambda N_{14}=0.25008\,\mathrm{Bq}
\simeq0.25\,\mathrm{Bq},}
$$

or approximately $15.0$ decays per minute per gram of carbon. A [becquerel](../../../../becquerel.md) is one decay per second; the normalization is per gram of carbon, rather than per gram of the entire organic sample.

**Artefact age**. Its remaining activity fraction is $0.13/0.25008=0.51983$. Inverting the [exponential decay](../../../../exponential-decay.md) law,

$$
\boxed{t=\frac{1}{\lambda}\ln\frac{\mathcal A_0}{\mathcal A}
=8266.64\,\mathrm{yr}\times\ln\frac{0.25008}{0.13}
=5408.44\,\mathrm{yr}\simeq5.4\times10^3\,\mathrm{yr}.}
$$

This is the [radiocarbon age](../../../../radiocarbon-age.md) on the supplied constant-initial-activity, $5730$-year [half-life](../../../../half-life.md) model. It is not a calibrated calendar date; the sample's historical initial ratio and any later carbon exchange are not supplied.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the particle and nuclear physics course of the University of Cambridge](../../../split.md)
5. [Particle and Nuclear Physics course of the University of Cambridge](../../../../particle-and-nuclear-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
