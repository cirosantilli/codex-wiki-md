# Independent spin Barnett response

↑ **Parent:** [Barnett effect](barnett-effect.md)

Consider an explicitly stipulated dilute [independent spin-one-half two-level system](independent-spin-one-half-two-level-system.md) with zero applied [magnetic field](magnetic-field-split.md). Each constituent has $J_z=\pm\hbar/2$ and $m_z=\gamma J_z$, with constant signed [gyromagnetic ratio](gyromagnetic-ratio.md) $\gamma$. Ignore interactions and the specimen's own [magnetic field](magnetic-field-split.md). At positive [temperature](temperature-split.md) $T$, [thermal equilibrium](thermal-equilibrium-split.md) with the rotating lattice gives [energy levels](energy-level.md) $E_\pm=\mp\hbar\Omega/2$. Define the dimensionless variable $x=\hbar\Omega/(2k_BT)$, where $\hbar$ is the [reduced Planck constant](reduced-planck-constant.md) and $k_B$ is the [Boltzmann constant](boltzmann-constant.md). The [partition function](canonical-partition-function.md) and [Boltzmann distribution](boltzmann-distribution.md) give

$$
Z=e^x+e^{-x}=2\cosh x,\qquad
p_+=\frac{e^x}{Z},\qquad p_-=\frac{e^{-x}}{Z}.
$$

Taking the [expected value](expected-value-split.md) gives

$$
\langle J_z\rangle=\frac\hbar2\tanh x,\qquad
\langle m_z\rangle=\gamma\frac\hbar2\tanh x,\qquad
M_z=n\gamma\frac\hbar2\tanh x,
$$

where $n$ is [number density](number-density.md). This is the rotational version of the [independent-moment magnetic response](independent-moment-magnetic-response.md). The [angular momentum](angular-momentum.md) aligns with positive rotation even when the [magnetic moment](magnetic-dipole-moment.md) points oppositely. The [probability](probability.md) ratio $p_+/p_-=e^{2x}$ provides a direct population check of the sign.

For $|x|\ll1$, expand the [hyperbolic tangent](hyperbolic-tangent.md) to obtain

$$
M_z\simeq\frac{n\gamma\hbar^2}{4k_BT}\Omega
=\frac{n\gamma^2\hbar^2}{4k_BT}B_\Omega.
$$

The slope against $B_\Omega$ is positive for either sign of $\gamma$, while the slope against $\Omega$ has the sign of $\gamma$. At fixed $T>0$, reversing $\Omega$ reverses both means, and $\Omega=0$ gives zero. At fixed nonzero $\Omega$, the formal $T\to0^+$ limit saturates $|\langle J_z\rangle|$ at $\hbar/2$; the linear approximation must not be extrapolated there. At $T\to\infty$, the response vanishes. These limits describe the toy [canonical ensemble](canonical-ensemble-split.md), whose equilibration is assumed.

<a id="image-signed-magnetic-moment-and-angular-momentum-response-to-rotation"></a>
![](barnett-independent-spin-rotation-response.png)

**[Figure 10](#image-signed-magnetic-moment-and-angular-momentum-response-to-rotation). Signed magnetic moment and angular momentum response to rotation**. Original calculated [Independent spin Barnett response](independent-spin-barnett-response.md), with $\gamma<0$. The left panel reaches the formal saturation limits; the right panel is the extremely small-polarization room-[temperature](temperature-split.md) regime. The stipulated inputs describe a toy collection of independent [spins](spin.md); neither panel represents measurements of a [ferromagnet](ferromagnet.md) or a fit to the gadolinium experiment.

For a numerical example, stipulate $n=10^{28}\,\mathrm{m^{-3}}$, $T=300\,\mathrm K$, $\gamma=-1.76\times10^{11}\,\mathrm{s^{-1}\,T^{-1}}$, and rotation [frequency](frequency.md) $f=1000\,\mathrm{Hz}$. With $\Omega=2\pi f$, $\hbar=1.054571817\times10^{-34}\,\mathrm{J\,s}$, and $k_B=1.380649\times10^{-23}\,\mathrm{J/K}$, the model gives

$$
B_\Omega=-35.7\,\mathrm{nT},\qquad
x=8.00\times10^{-11},\qquad
M_z=-7.42\times10^{-6}\,\mathrm{A/m}.
$$

These are teaching inputs and calculated outputs, not measured material values. The corresponding internal [angular momentum](angular-momentum.md) density is $M_z/\gamma=+4.22\times10^{-17}\,\mathrm{J\,s/m^3}$. Keeping a rotor at prescribed $\Omega$ while its internal [angular momentum](angular-momentum.md) changes requires the drive to supply the appropriate angular [impulse](impulse.md). In an isolated body the mechanical part instead changes oppositely, as in [magnetomechanical angular momentum balance](magnetomechanical-angular-momentum-balance.md). There is no creation of net [angular momentum](angular-momentum.md) by choosing a rotating frame.

## ↑ Ancestors (7)

1. [Barnett effect](barnett-effect.md)
2. [Magnetic dipole moment](magnetic-dipole-moment.md)
3. [Magnetic vector potential](magnetic-vector-potential.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Independent spin Barnett response](independent-spin-barnett-response.md)
