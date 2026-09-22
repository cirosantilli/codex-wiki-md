# Delayed-pumping model of Sisyphus friction

↑ **Parent:** [Sisyphus cooling](sisyphus-cooling.md)

Consider an original reduced [rate equation](rate-equation.md) model using the same potentials. Write $s(z)=\cos(2kz)$ and stipulate positive [optical pumping](optical-pumping.md) rates $R_{+\to-}=\gamma_p(1-s)$, $R_{-\to+}=\gamma_p(1+s)$, with $\gamma_p>0$. They pump towards $+$ at $z=0$ and towards $-$ at $z=\lambda/4$, consistently with the diagram. These rates retain the relevant symmetry and delay, while omitting excited-state dynamics, [quantum coherence](quantum-coherence-in-a-specified-basis.md) and recoil diffusion.

For populations $p_++p_-=1$, put $q=p_+-p_-$. The [rate equations](rate-equation.md) conserve population and give $\dot q=2\gamma_p(s-q)$. The stationary atom has $q=s$; a moving atom cannot follow it instantaneously. On a prescribed trajectory $z=vt$, the periodic solution is

$$
q(z)=\frac{\gamma_p^2\cos(2kz)+\gamma_pkv\sin(2kz)}{\gamma_p^2+k^2v^2}.
$$

Substitution into $vq'=2\gamma_p(s-q)$ verifies both coefficients. The mean mechanical [force](force-split.md) is $F=-p_+U_+'-p_-U_-'=-U_0kq\sin(2kz)$. Averaging over a spatial period, with mean squared sine $1/2$ and mean sine times cosine zero, gives

$$
\overline F=-\frac{U_0k^2v\gamma_p}{2(\gamma_p^2+k^2v^2)},\qquad
\overline F\simeq-\frac{U_0k^2}{2\gamma_p}v\quad (|kv|\ll\gamma_p).
$$

Thus the [force](force-split.md) opposes either sign of [velocity](velocity.md) and vanishes at rest. A small pumping rate makes the small-[velocity](velocity.md) friction slope large while narrowing its useful [velocity](velocity.md) range. Holding $v$ fixed while sending $\gamma_p$ to zero makes the [force](force-split.md) vanish; the apparently divergent zero-[velocity](velocity.md) slope is not unlimited cooling. Because this model has no [momentum](momentum-split.md) diffusion, it predicts no equilibrium [temperature](temperature-split.md). It demonstrates the lag mechanism rather than replacing a multilevel quantum calculation.

## ↑ Ancestors (8)

1. [Sisyphus cooling](sisyphus-cooling.md)
2. [Polarization-gradient cooling](polarization-gradient-cooling.md)
3. [Sub-Doppler cooling](sub-doppler-cooling.md)
4. [Laser cooling](laser-cooling.md)
5. [Atomic measurement methods](atomic-measurement-methods.md)
6. [Atomic physics](atomic-physics-split.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
