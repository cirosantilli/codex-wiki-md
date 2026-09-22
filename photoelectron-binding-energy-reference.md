# Photoelectron binding energy reference

↑ **Parent:** [X-ray photoelectron spectroscopy](x-ray-photoelectron-spectroscopy.md)

Let a conducting sample and conducting analyzer be in good electrical contact, unbiased, at equilibrium, and without appreciable charging during illumination. Their [Fermi levels](fermi-level.md) then coincide. Choose that common [Fermi level](fermi-level.md) as zero. Define $E_B>0$ as the [binding energy](binding-energy.md) relative to this zero: removing an [electron](electron.md) into the [electron](electron.md) reservoir at the [Fermi level](fermi-level.md) costs $E_B$. It is not the cost of removing the [electron](electron.md) all the way to the sample's [vacuum](vacuum.md) level.

Write the sample and analyzer [work functions](work-function.md) as $\phi_s$ and $\phi_a$. Their local [vacuum](vacuum.md) levels lie at $\phi_s$ and $\phi_a$ above the common [Fermi level](fermi-level.md). [Conservation of energy](conservation-of-energy.md) for an [electron](electron.md) emitted without additional losses gives total outgoing [energy](energy-split.md) $h\nu-E_B$, where $h$ is the [Planck constant](planck-constant.md) and $\nu$ the [photon](photon.md) [frequency](frequency.md). Immediately outside the sample its [kinetic energy](kinetic-energy.md) is $K_s=h\nu-E_B-\phi_s$. The contact-related [electric potential](electric-potential.md) changes this to

$$
E_{\rm kin}=K_s+\phi_s-\phi_a
=h\nu-E_B-\phi_a,
\qquad
E_B=h\nu-E_{\rm kin}-\phi_a.
$$

Thus the sample [work function](work-function.md) cancels when the measured [kinetic energy](kinetic-energy.md) is referenced to the analyzer. Substituting $\phi_s$ for $\phi_a$ in the final conversion would mix two different [energy](energy-split.md) references. An instrument's calibrated [binding energy](binding-energy.md) scale can incorporate its effective analyzer [work function](work-function.md), so the correction need not appear as a separate operator-entered number.

As an original numerical example, stipulate $h\nu=1486.6\,\mathrm{eV}$, $\phi_a=4.5\,\mathrm{eV}$ and a line at $E_B=284.0\,\mathrm{eV}$. The predicted analyzer [kinetic energy](kinetic-energy.md) is $1198.1\,\mathrm{eV}$. If $\phi_s=5.0\,\mathrm{eV}$, the surface value is instead $K_s=1197.6\,\mathrm{eV}$; the contact-related increase is $0.5\,\mathrm{eV}$. A second line at $286.0\,\mathrm{eV}$ gives $1196.1\,\mathrm{eV}$ at the analyzer. A $+2.0\,\mathrm{eV}$ [chemical shift in photoelectron spectroscopy](chemical-shift-in-photoelectron-spectroscopy.md) therefore appears as a $-2.0\,\mathrm{eV}$ shift in measured [kinetic energy](kinetic-energy.md). These are chosen values, not a measured [carbon](carbon.md) spectrum.

Charging breaks the assumed reference. If a uniformly charging sample rises by [electric potential](electric-potential.md) $V>0$ relative to the analyzer, an escaping [electron](electron.md) loses an additional [energy](energy-split.md) $eV$, with $e$ the positive [elementary charge](elementary-charge.md). Applying the unbiased conversion consequently returns

$$
E_{B,\mathrm{apparent}}=E_{B,\mathrm{true}}+eV.
$$

Two features from the same stable potential retain their separation. Features from regions at different potentials acquire different offsets, which can mimic chemical differences or broaden a line. A conducting holder alone does not establish electrical contact through an insulating surface layer. Compare repeat scans, electrical contact and charge-compensation settings before interpreting an offset as a change in [chemical bonds](chemical-bond-split.md).

[Measurement calibration](measurement-calibration.md) is a separate issue: a known reference line tests the scale, while charge compensation controls the specimen's [electric potential](electric-potential.md). In an original offset model $E_{B,\mathrm{read}}=E_{B,\mathrm{true}}+b$, one known line determines $b$. An unknown scale factor in $E_{B,\mathrm{read}}=aE_{B,\mathrm{true}}+b$ requires two distinct known lines to determine both $a$ and $b$. Re-reading a reference after a sample checks drift. Treating an unidentified contamination peak as a universally fixed reference would assume the chemical identity and electrical behavior that the measurement should test.

## ↑ Ancestors (5)

1. [X-ray photoelectron spectroscopy](x-ray-photoelectron-spectroscopy.md)
2. [Photoemission spectroscopy](photoemission-spectroscopy.md)
3. [Physical chemistry](physical-chemistry-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Chemical shift in photoelectron spectroscopy](chemical-shift-in-photoelectron-spectroscopy.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2018/section-b/b4/solution.md)
- [Photoemission spectroscopy](photoemission-spectroscopy.md)
- [Siegbahn photoelectron spectroscopy experiments](siegbahn-photoelectron-spectroscopy-experiments.md)
