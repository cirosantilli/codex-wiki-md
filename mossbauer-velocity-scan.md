<h1 id="mossbauer-velocity-scan">Mössbauer velocity scan</h1>

↑ **Parent:** [Mössbauer effect](mossbauer-effect-split.md)

Let $v$ be the source [velocity](velocity.md) towards the absorber, positive for approach along the [photon](photon.md) direction. A first-order [Lorentz transformation](lorentz-transformation.md) of the [photon](photon.md) [energy](energy-split.md) gives $E'=E+vp$; hence, for $|v|\ll c$,

$$
\delta E\simeq E_\gamma\frac{v}{c}.
$$

Moving the source shifts its [emission line](emission-line.md) through the stationary [absorption line](absorption-line.md). A minimum in transmitted [photon](photon.md) counts marks their strongest overlap. The absorber is the narrow [energy](energy-split.md) discriminator; the downstream [particle detector](particle-detector.md) only needs to count the transmitted [gamma rays](gamma-ray.md).

For a thin absorber with unsplit [Lorentzian line shapes](lorentzian-line-shape.md), the overlap is a [convolution](convolution.md) of the source and absorber profiles. The combined [full width at half maximum](full-width-at-half-maximum.md) is $W=\Gamma_s+\Gamma_a$. A simple expected transmission model is

$$
\frac{I(v)}{I_0}=1-\frac{A}{1+\left[2E_\gamma(v-v_0)/(cW)\right]^2},\qquad 0<A<1.
$$

Here $I_0$ is the off-resonance intensity, $v_0$ encodes a relative shift of the two transition [energies](energy-split.md), and $A$ includes the resonant absorber strength and $f_s f_a$. The convolution result can be checked by multiplying the [Fourier transforms](fourier-transform-split.md) of two [Cauchy distributions](cauchy-distribution.md): their exponential decay constants add. The width of the absorption dip in [velocity](velocity.md) is $cW/E_\gamma$, rather than the width of one individual [spectral line](spectral-line.md) converted to [velocity](velocity.md).

For the teaching system with $\Gamma_s=\Gamma_a=\Gamma_E$ and $v_0=0$, the dip's [full width at half maximum](full-width-at-half-maximum.md) is $2.9979\,\mathrm{mm\,s^{-1}}$. Stipulate $A=0.25$ at zero [temperature](temperature-split.md) and $10{,}000$ expected off-resonance counts per equal-duration bin: the central bin then has $7{,}500$ expected counts, and the half-depth bins have $8{,}750$. These are model expectations, without sampled counting noise. Holding all other parameters fixed while heating both lattices to $k_BT=2\hbar\omega$ multiplies $A$ by $[f(T)/f(0)]^2$. This isolates how a falling [recoil-free fraction](lamb-mossbauer-factor.md) weakens the dip.

<a id="image-mechanical-velocity-scans-an-absorption-line-much-narrower-than-detector-resolution"></a>
![](mossbauer-resonant-absorption-velocity-scan.png)

**[Figure 2](#image-mechanical-velocity-scans-an-absorption-line-much-narrower-than-detector-resolution). Mechanical velocity scans an absorption line much narrower than detector resolution**. Original ideal transmission model, with schematic source, absorber and counting detector. Both curves use the same stipulated [energy](energy-split.md) widths; heating changes only $f_s f_a$. Dashed markers show the cold curve's half-depth positions. This is a new analytic teaching scan, not a historical measurement or a fit. The upper scale converts [velocity](velocity.md) to [Doppler effect](doppler-effect.md) [energy](energy-split.md) shift.

The thin-absorber model is deliberately limited. A thick absorber can saturate and broaden the dip; unresolved [hyperfine structure](hyperfine-structure.md) can create multiple components. Differences in chemical surroundings can shift the centers, and uncontrolled motion can smear them. These effects must be modeled before interpreting an observed width as a [natural linewidth](natural-linewidth.md). Their sensitivity also makes the [Mössbauer effect](mossbauer-effect-split.md) useful: a small displacement of a narrow dip can reveal a small change in the local nuclear environment.

## ↑ Ancestors (4)

1. [Mössbauer effect](mossbauer-effect-split.md)
2. [Nuclear physics](nuclear-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)
