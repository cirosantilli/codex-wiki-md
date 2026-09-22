# Shockley diode equation

↑ **Parent:** [Diode](diode.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shockley_diode_equation)

For a [p-n junction](p-n-junction.md) at fixed [temperature](temperature-split.md), the [Shockley diode equation](shockley-diode-equation.md) models its [electric current](electric-current.md) as

$$
I_D=I_S\left(\exp\frac{V_D}{nV_T}-1\right),\qquad V_T=\frac{k_BT}{q}.
$$

Here $I_S>0$ is the [diode saturation current](diode-saturation-current.md), $n>0$ the [diode ideality factor](diode-ideality-factor.md), $V_T$ the [thermal voltage](thermal-voltage.md), $k_B$ the [Boltzmann constant](boltzmann-constant.md), and $q>0$ the [elementary charge](elementary-charge.md).[The Junction Diode, §1.2, printed p. 4, equation (1.1) and parameter definitions](the-junction-diode-by-w-marshall-leach-jr.md)

For an original model example, choose $I_S=1\,\mathrm{nA}$, $n=2$, and $T=300\,\mathrm K$. Using $k_B=1.380649\times10^{-23}\,\mathrm{J/K}$ and $q=1.602176634\times10^{-19}\,\mathrm C$ gives $V_T=25.8520\,\mathrm{mV}$. Then $V_D=0.600\,\mathrm V$ gives $I_D=0.109591\,\mathrm{mA}$, whereas $V_D=0.800\,\mathrm V$ gives $I_D=5.24450\,\mathrm{mA}$. These are predictions of the declared model. There is no universal turn-on [electric potential difference](electric-potential-difference.md): solving the [Shockley diode equation](shockley-diode-equation.md) for the value needed at a chosen [electric current](electric-current.md) gives

$$
V_D=nV_T\ln\left(1+\frac{I_D}{I_S}\right),\qquad I_D>-I_S.
$$

At $I_D\gg I_S$, increasing $V_D$ by $0.100\,\mathrm V$ multiplies the [electric current](electric-current.md) by approximately $e^{0.100/(nV_T)}=6.91772$. At $V_D=-0.300\,\mathrm V$ the same model gives $I_D=-0.996979\,\mathrm{nA}$. Its reverse branch approaches $-I_S$; it cannot describe [diode reverse breakdown](diode-reverse-breakdown.md).

A constructed extension adds internal series [electrical resistance](electrical-resistance.md) $R_s$ to a junction whose [electric potential difference](electric-potential-difference.md) is $V_j$. Applying the [Kirchhoff cycle law](kirchhoff-cycle-law.md) gives

$$
V_D=V_j+I_DR_s
=nV_T\ln\left(1+\frac{I_D}{I_S}\right)+I_DR_s.
$$

For $R_s=20\,\Omega$ and the same $I_S,n,T$, sustaining $I_D=5.24450\,\mathrm{mA}$ needs $V_D=0.904890\,\mathrm V$: $0.800\,\mathrm V$ across the junction plus $0.104890\,\mathrm V$ across its internal [electrical resistance](electrical-resistance.md). The [derivative](derivative.md)

$$
\frac{dV_D}{dI_D}=\frac{nV_T}{I_D+I_S}+R_s
$$

shows why the [current-voltage characteristic](current-voltage-characteristic.md) becomes nearly a [straight line](straight-line.md) when the internal series [electrical resistance](electrical-resistance.md) dominates. This is still a fixed-[temperature](temperature-split.md) model; self-heating can change $I_S$, $n$ and $V_T$. Real [diodes](diode.md) also have leakage and charge-storage effects omitted here.[The Junction Diode, §§1.3, 1.8 and 1.11: temperature dependence, charge storage and series bulk resistance](the-junction-diode-by-w-marshall-leach-jr.md)

**Table of contents**

- [Diode minority-carrier diffusion current](diode-minority-carrier-diffusion-current.md)
- [Thermal voltage](thermal-voltage.md)
- [Diode saturation current](diode-saturation-current.md)
  - [Extracting a semiconductor band gap from diode saturation current](extracting-a-semiconductor-band-gap-from-diode-saturation-current.md)
- [Diode ideality factor](diode-ideality-factor.md)

## ↑ Ancestors (6)

1. [Diode](diode.md)
2. [Electrical circuit](electrical-circuit-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Blue light-emitting diode](blue-light-emitting-diode.md)
- [Diode](diode.md)
- [Diode characteristic measurement](diode-characteristic-measurement.md)
- [Diode ideality factor](diode-ideality-factor.md)
- [Diode reverse breakdown](diode-reverse-breakdown.md)
- [Diode saturation current](diode-saturation-current.md)
- [Esaki tunnel-diode experiment](esaki-tunnel-diode-experiment.md)
- [Ideal diode model](ideal-diode-model.md)
- [P-n junction](p-n-junction.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1/section-d/d13/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2/section-d/d13/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2/section-d/d12/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2005/section-b/b4/c/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2014/4/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2018/section-b/b2/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2021/section-b/6/c/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2022/section-b/6/d/solution.md)
- [Shockley diode equation](shockley-diode-equation.md)
- [Tunnel diode](tunnel-diode.md)
