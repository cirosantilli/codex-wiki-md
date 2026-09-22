# Electronic contrast in scanning tunneling microscopy

↑ **Parent:** [Scanning tunneling microscopy](scanning-tunneling-microscopy.md)

Separate geometry from electronic response in an original one-dimensional toy [tunnel junction](tunnel-junction.md). Write the geometric surface height as $h(x)$, tip height as $z(x)$, and positive gap as $s(x)=z(x)-h(x)$. Assume low fixed tip-sample [electric potential difference](electric-potential-difference.md): the sampled [energy](energy-split.md) window is narrow enough that the tip [density of states](density-of-states.md) is featureless and the sample [local density of states](local-density-of-states.md) varies little across that window. Neglect thermal broadening, changes of tip shape and lateral averaging. Let $\rho(x)>0$ be the effective sample [local density of states](local-density-of-states.md) divided by a positive reference value, so it is dimensionless. Choose a spatially constant effective barrier [energy](energy-split.md) $\Phi>0$, a positive coefficient $C$ with units of [electric current](electric-current.md), and

$$
I(x,z)=C\rho(x)\exp\bigl[-2\kappa(z-h(x))\bigr],\qquad
\kappa=\frac{\sqrt{2m_e\Phi}}{\hbar}>0.
$$

Here $m_e$ is the [electron](electron.md) [mass](mass.md), $\hbar$ the reduced [Planck constant](planck-constant.md), and $\kappa$ the [tunnelling decay constant](tunnelling-decay-constant.md). This is an illustrative low-bias model, not a universal calibration formula. At fixed $I=I_0>0$, taking a [logarithm](logarithm.md) gives

$$
\ln(I_0/C)=\ln\rho-2\kappa(z-h),\qquad
z(x)=h(x)+\frac{\ln\rho(x)}{2\kappa}+s_0,\qquad
s_0=\frac{\ln(C/I_0)}{2\kappa}.
$$

The [logarithms](logarithm.md) have dimensionless arguments. Only constant $\rho$ makes the recorded height differ from geometric height by a constant. Multiplying $\rho$ by $r>0$ raises the apparent height by $\ln r/(2\kappa)$ without moving the geometric surface.

For a concrete ambiguity, choose $\kappa=10\,\mathrm{nm}^{-1}$, $a=0.020\,\mathrm{nm}$, lateral period $L=1\,\mathrm{nm}$, $s_0=0.50\,\mathrm{nm}$, and $q(x)=\cos(2\pi x/L)$. Compare

$$
\begin{aligned}
h_A(x)&=a q(x),&\rho_A(x)&=1,\\
h_B(x)&=0,&\rho_B(x)&=\exp\bigl(2\kappa a q(x)\bigr).
\end{aligned}
$$

Both produce exactly $z(x)=s_0+a q(x)$ at $I_0=C e^{-2\kappa s_0}=C e^{-10}$. Substitution checks this without identifying $\rho$ with geometric height: case A has constant gap $s_0$, while case B has gap $s_0+a q(x)$ and a compensating electronic factor. The chosen $\rho_B$ ranges from $e^{-0.4}$ to $e^{0.4}$, approximately $0.6703$ to $1.4918$; every gap remains positive. The chosen $\kappa$ corresponds to $\Phi\simeq3.81$ [electronvolts](electronvolt.md), a positive effective barrier.

At fixed tip height $z_f=s_0$, both cases instead give

$$
\frac{I(x,z_f)}{I_0}=\exp\bigl[0.4q(x)\bigr].
$$

Their maximum-to-minimum [electric current](electric-current.md) ratio is $e^{0.8}\simeq2.226$. Thus even adding this fixed-height scan at the same [electric potential difference](electric-potential-difference.md) cannot distinguish these deliberately chosen surfaces within the toy model. Independent structural information or additional electronic measurements are required. Changing [electric potential difference](electric-potential-difference.md) can supply such information, but also changes the assumptions used to define $C$ and $\rho$.

<a id="image-different-geometric-and-electronic-profiles-can-produce-the-same-stm-image"></a>
![](scanning-tunneling-height-electronic-contrast.png)

**[Figure 18](#image-different-geometric-and-electronic-profiles-can-produce-the-same-stm-image). Different geometric and electronic profiles can produce the same STM image**. Original toy calculations, not measured data. The corrugated surface with constant [local density of states](local-density-of-states.md) and the flat surface with varying [local density of states](local-density-of-states.md) give identical recorded heights under [constant-current scanning tunneling microscopy](constant-current-scanning-tunneling-microscopy.md). They also give identical fixed-height [electric current](electric-current.md) contrast at this chosen bias.

## ↑ Ancestors (8)

1. [Scanning tunneling microscopy](scanning-tunneling-microscopy.md)
2. [Tunnel junction](tunnel-junction.md)
3. [Quantum tunnelling](quantum-tunnelling.md)
4. [Potential barrier](potential-barrier.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Constant-current scanning tunneling microscopy](constant-current-scanning-tunneling-microscopy.md)
- [Scanning tunneling microscope](scanning-tunneling-microscope.md)
