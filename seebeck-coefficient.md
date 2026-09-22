# Seebeck coefficient

↑ **Parent:** [Seebeck effect](seebeck-effect.md)

The [Seebeck coefficient](seebeck-coefficient.md) $S(T)$ quantifies the thermoelectric voltage response per small [temperature](temperature.md) difference at zero [electric current](electric-current.md). Use $S=-dV/dT$ along a homogeneous material, with voltage understood through [electrochemical potential](electrochemical-potential.md). Its units are [volts](volt.md) per [kelvin](kelvin.md), commonly $\mu\mathrm{V/K}$. The word [thermopower](seebeck-coefficient.md) is also used, despite this being a voltage response rather than [power](power.md); some authors use that word for $|S|$, so check their convention. [Northwestern thermoelectrics research group: Seebeck coefficient and thermopower convention](https://thermoelectrics.matsci.northwestern.edu/thermoelectrics/).

For the A-minus-B terminal order in the [Seebeck effect](seebeck-effect.md) experiment,

$$
\frac{\partial V_{AB}}{\partial T_h}=S_A(T_h)-S_B(T_h),\qquad
\frac{\partial V_{AB}}{\partial T_c}=-\bigl[S_A(T_c)-S_B(T_c)\bigr].
$$

Thus a small [temperature](temperature.md) difference around $T_0$ gives $V_{AB}\approx[S_A(T_0)-S_B(T_0)]\Delta T$. The finite-interval ratio $V_{AB}/\Delta T$ is an average of the coefficient difference, not necessarily its value at either endpoint. Ordinary two-material measurements determine a relative [Seebeck coefficient](seebeck-coefficient.md): to recover $S_A$ from the measured difference, add a separately known $S_B$. Neither the choice of a zero for voltage nor the use of a familiar reference material makes $S_B$ identically zero.

A concrete research example is Martin and colleagues' 2021 certification experiment. They measured small [temperature](temperature.md) differences and voltages on six [silicon](silicon.md)–germanium specimens at 13 base [temperatures](temperature.md) between $295$ and $900\,\mathrm K$. At each setting they acquired 40 voltage-and-[temperature](temperature.md)-difference pairs and used [linear regression](linear-regression-split.md) with a free intercept, so a constant voltage offset did not become part of the [slope](slope.md). Platinum voltage leads required a reference-material correction; their terminal order gave $S_{\rm measured}=S_{\rm Pt}-S_{\rm specimen}$, hence $S_{\rm specimen}=S_{\rm Pt}-S_{\rm measured}$. This is an actual measurement protocol, unlike the toy plot above. [Martin et al., Development of a high-temperature (295–900 K) Seebeck coefficient Standard Reference Material (2021), certification measurements and Eq. (1)](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=932592).

Microscopically, a [temperature gradient](temperature-gradient.md) changes [charge carrier](charge-carrier.md) transport until an opposing electrical response balances it at zero net [electric current](electric-current.md). In the usual simple [semiconductor](semiconductor.md) picture, [Electrons](electron.md) and [electron holes](electron-hole.md) give opposite [Seebeck coefficient](seebeck-coefficient.md) signs, and their contributions are weighted by their [electrical conductivities](electrical-conductivity.md). The [Seebeck coefficient](seebeck-coefficient.md) is a transport property: [density of states](density-of-states.md) alone does not determine it, since carrier motion and scattering also matter. Its usefulness extends beyond [temperature](temperature.md) sensing to diagnosing which carriers transport [electric charge](electric-charge.md). [Northwestern thermoelectrics research group: Seebeck coefficient, scattering contributions, and bipolar transport](https://thermoelectrics.matsci.northwestern.edu/thermoelectrics/).

## ↑ Ancestors (6)

1. [Seebeck effect](seebeck-effect.md)
2. [Thermoelectric effect](thermoelectric-effect.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/33b/solution.md)
- [Seebeck coefficient](seebeck-coefficient.md)
- [Seebeck effect](seebeck-effect.md)
- [Thermocouple](thermocouple.md)
