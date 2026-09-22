<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $n_{56}$ and $n_{54}$ for the number densities of nickel-56 and iron-54. Both nuclei contain 28 [neutrons](../../../../../../neutron.md), while their [proton](../../../../../../proton.md) numbers differ by two. Dividing the positive-exponential [nuclear statistical equilibrium](../../../../../../nuclear-statistical-equilibrium.md) formulas printed in the PDF therefore gives the [nickel–iron nuclear equilibrium ratio](../../../../../../nickel-iron-nuclear-equilibrium-ratio.md)

$$
\boxed{\frac{n_{56}}{n_{54}}=K n_p^2T^{-3}
\exp\left(\frac{\Delta Q}{kT}\right),\qquad
\Delta Q=Q(56,28)-Q(54,26).}
$$

The neutron-density factors cancel. $K$ contains the isotope-dependent statistical and translational [mass](../../../../../../mass.md) factors suppressed in the supplied proportionality; it is constant in this simplified calculation. The TeX conversion incorrectly reverses the exponential sign, so the PDF sign is essential here.

In the specified restricted composition, equality of total [proton](../../../../../../proton.md) and [neutron](../../../../../../neutron.md) numbers means

$$
28n_{56}+26n_{54}+n_p=28n_{56}+28n_{54},
\qquad\boxed{n_p=2n_{54}.}
$$

Consequently

$$
F(T)=\frac{n_{56}}{n_{54}^3}=4K T^{-3}e^{\Delta Q/(kT)}.
$$

Differentiation, with the suppressed prefactors held constant, gives

$$
\frac{d\log F}{dT}=-\frac3T-\frac{\Delta Q}{kT^2}.
$$

Using the paper's supplied signed energy difference produces

$$
\boxed{T_{\max}=-\frac{\Delta Q}{3k}=9.0\times10^9\ \mathrm K.}
$$

With that negative value, $F$ tends to zero at both [temperature](../../../../../../temperature.md) endpoints, increases below this [temperature](../../../../../../temperature.md) and decreases above it. At the stationary point $d^2\log F/dT^2=-3/T^2<0$, so it is indeed a maximum for the printed toy data.

There is a genuine physical-data qualification: the stated negative energy difference is inconsistent with interpreting $Q$ as the conventional positive total [nuclear binding energy](../../../../../../nuclear-binding-energy.md) of these actual isotopes. Using atomic masses, whose electron masses cancel in this reaction,

$$
\Delta B\simeq[2m({}^1\mathrm H)+m({}^{54}\mathrm{Fe})-m({}^{56}\mathrm{Ni})]c^2
\simeq+12.23\ \mathrm{MeV}>0.
$$

The masses used are $1.00782503223\,\mathrm u$, $53.93960899\,\mathrm u$ and $55.94212855\,\mathrm u$, from [NIST hydrogen masses](https://physics.nist.gov/cgi-bin/Compositions/stand_alone.pl?ele=H&isotype=all), [NIST iron masses](https://physics.nist.gov/cgi-bin/Compositions/stand_alone.pl?ele=Fe&isotype=all) and [NIST nickel masses](https://physics.nist.gov/cgi-bin/Compositions/stand_alone.pl?ele=Ni&isotype=all). Small electronic binding corrections do not change the sign. With a positive $\Delta B$, the simplified $F(T)$ above is strictly decreasing for $T>0$ and has no finite maximum. Thus the numerical maximum follows from the supplied negative parameter, not from consistent physical binding energies; changing the TeX sign to recover a maximum would not repair the PDF's data.

[Nuclear statistical equilibrium](../../../../../../nuclear-statistical-equilibrium.md) is appropriate when the relevant forward and inverse strong or electromagnetic reactions are fast compared with changes of [temperature](../../../../../../temperature.md), density and composition. It is useful in sufficiently hot late silicon-burning material and in the hottest explosive burning regions of massive stars. Some burning zones reach only quasi-equilibrium, and cooling or expansion eventually freezes the abundances out; an equilibrium expression cannot by itself predict the full ashes when these timescale conditions fail. [Temperature](../../../../../../temperature.md), density, conserved [baryon number](../../../../../../baryon-number.md) and the [electron fraction in stellar matter](../../../../../../electron-fraction-in-stellar-matter.md) must all be specified. Negligible free-particle contributions in bulk bookkeeping are not the same as exactly zero free densities in the equilibrium formula.

Strong and electromagnetic reactions preserve total charge and [baryon number](../../../../../../baryon-number.md), so they conserve the proton-to-neutron ratio. Weak reactions need not: [electron capture](../../../../../../electron-capture.md) and [beta-plus decay](../../../../../../beta-plus-decay.md) convert [protons](../../../../../../proton.md) into [neutrons](../../../../../../neutron.md) and lower it. Such conversions occur in hydrogen-burning networks and in the nitrogen-to-neon chain during [helium](../../../../../../helium.md) burning. At high density in advanced stellar cores and core collapse, [electron capture](../../../../../../electron-capture.md) becomes particularly important; [neutrino](../../../../../../neutrino.md) emission also affects energy and lepton loss. [Beta-minus decay](../../../../../../beta-minus-decay.md) changes the ratio in the opposite direction and can compete during later relaxation. Nuclear equilibrium for strong reactions does not automatically imply weak equilibrium or a fixed proton-to-neutron ratio throughout all [stellar evolution](../../../../../../stellar-evolution.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
