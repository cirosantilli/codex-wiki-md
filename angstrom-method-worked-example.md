<h1 id="angstrom-method-worked-example">Ångström method worked example</h1>

↑ **Parent:** [Ångström periodic heating method](angstrom-periodic-heating-method.md)

Consider an original stipulated model, not measured material data: [thermal diffusivity](thermal-diffusivity.md) $\alpha=10^{-4}\,\mathrm{m^2\,s^{-1}}$, period $P=100\,\mathrm s$, driven [temperature](temperature-split.md) [amplitude](wave-amplitude.md) $\Theta_0=4\,\mathrm K$, and [thermometers](thermometer.md) at $x_1=0.020\,\mathrm m$ and $x_2=0.050\,\mathrm m$. Without side losses, $a=b=17.7245\,\mathrm{m^{-1}}$ and [thermal penetration depth](thermal-penetration-depth.md) $\delta=0.05642\,\mathrm m$. Thus

$$
A_1=2.80612\,\mathrm K,\quad A_2=1.64883\,\mathrm K,\quad
D=\Delta\phi=0.531736,\quad\Delta t=8.46284\,\mathrm s.
$$

The two no-loss estimates and the combined estimate all return $10^{-4}\,\mathrm{m^2\,s^{-1}}$.

Now retain the same [thermal diffusivity](thermal-diffusivity.md) and drive but introduce $\lambda=0.010\,\mathrm{s^{-1}}$. The exact [complex wavenumber](complex-wavenumber.md) gives $a=19.1863\,\mathrm{m^{-1}}$ and $b=16.3742\,\mathrm{m^{-1}}$, hence

$$
\begin{aligned}
A_1&=2.72527\,\mathrm K,& A_2&=1.53262\,\mathrm K,\\
D&=0.575588,&\Delta\phi&=0.491225\,\mathrm{rad},\\
\Delta t&=7.81809\,\mathrm s,&\alpha_{\rm combined}&=10^{-4}\,\mathrm{m^2\,s^{-1}}.
\end{aligned}
$$

Using attenuation alone with the no-loss formula would give $8.5343\times10^{-5}\,\mathrm{m^2\,s^{-1}}$; using lag alone would give $1.17174\times10^{-4}\,\mathrm{m^2\,s^{-1}}$. Their disagreement is informative. If an independent [volumetric heat capacity](volumetric-heat-capacity.md) measurement gives $\rho c_p=2.0\times10^6\,\mathrm{J\,m^{-3}\,K^{-1}}$, the combined estimate implies [thermal conductivity](thermal-conductivity.md) $k=200\,\mathrm{W\,m^{-1}\,K^{-1}}$ and $H=2.0\times10^4\,\mathrm{W\,m^{-3}\,K^{-1}}$.

<a id="image-solved-angstrom-method-example-spatial-amplitude-wave-phase-lag-time-traces-and-finite-end-bias"></a>
![](angstrom-periodic-heating-amplitude-phase.png)

**[Figure 6](#image-solved-angstrom-method-example-spatial-amplitude-wave-phase-lag-time-traces-and-finite-end-bias). Solved Ångström method example: spatial amplitude, wave phase lag, time traces and finite-end bias**. Original analytical predictions using the stipulated parameters above. Dots in the upper panels independently solve the spatial [heat equation](heat-equation.md) with [finite differences](finite-difference-split.md). The lower-left traces show the linear-loss case at the two sensor positions. The lower-right curve applies the semi-infinite inference to an exact finite rod with an insulated far end: the resulting apparent [thermal diffusivity](thermal-diffusivity.md) can lie above or below the true value. None of these curves are experimental data.

The exact [complex amplitudes](complex-amplitude.md) can be checked independently by discretizing $\alpha\widehat\theta''-(\lambda+i\omega)\widehat\theta=0$ and solving the resulting [linear system](system-of-linear-equations.md) with a [tridiagonal matrix](tridiagonal-matrix.md). Halving the spatial step quarters the discrepancy, as expected for centered [finite differences](finite-difference-split.md). Separately fitting the real time traces to a constant plus [sine](sine.md) and [cosine](cosine.md) terms recovers both [amplitudes](wave-amplitude.md) and their lag; this also checks the sign convention used in the combined estimate.

## ↑ Ancestors (9)

1. [Ångström periodic heating method](angstrom-periodic-heating-method.md)
2. [Thermal diffusivity](thermal-diffusivity.md)
3. [Thermal conduction](thermal-conduction.md)
4. [Heat](heat-split.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Finite-end correction for periodic rod heating](finite-end-correction-for-periodic-rod-heating.md)
