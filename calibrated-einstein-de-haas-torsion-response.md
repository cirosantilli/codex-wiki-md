# Calibrated Einstein-de Haas torsion response

↑ **Parent:** [Einstein-de Haas effect](einstein-de-haas-effect.md)

An original reduced model makes the calibration explicit. Let the [torsion pendulum](torsion-pendulum.md) have restoring [torque](torque.md) $-\kappa\theta$, with [torsion constant](torsion-constant.md) $\kappa$, and [viscous damping](viscous-damping.md) [torque](torque.md) $-b\dot\theta$, with $b>0$. Allow an unwanted axial [torque](torque.md) $\tau_p(t)$:

$$
I\ddot\theta+b\dot\theta+\kappa\theta
=-\frac{\dot m_z}{\gamma}+\tau_p(t),\qquad
\omega_0=\sqrt{\frac{\kappa}{I}},\qquad
Q=\frac{I\omega_0}{b}.
$$

Here $\omega_0$ is the undamped natural [angular frequency](angular-frequency.md) and $Q$ the [quality factor](q-factor.md). The [forced harmonic oscillator](forced-harmonic-oscillator.md) response must be included before a twist can be interpreted as a [torque](torque.md).

Using the [complex amplitude](complex-amplitude.md) convention $m_z(t)=\operatorname{Re}(\widetilde m e^{\mathrm i\omega t})$ and similarly for $\theta$ and $\tau_p$, differentiation multiplies by $\mathrm i\omega$. Substitution gives

$$
H_\tau(\omega)=\frac{1}{\kappa-I\omega^2+\mathrm i b\omega},
\qquad
\widetilde\theta=H_\tau(\omega)
\left(-\frac{\mathrm i\omega}{\gamma}\widetilde m+\widetilde\tau_p\right).
$$

This is the torque-to-twist [transfer function](transfer-function.md). With $\widetilde\tau_p=0$ and real positive $\widetilde m=m_1$, the twist [amplitude](wave-amplitude.md) is

$$
A_{\rm EdH}(\omega)=\frac{\omega m_1/|\gamma|}{\sqrt{(\kappa-I\omega^2)^2+(b\omega)^2}}.
$$

For $\gamma<0$, the twist [phase](phase-waves.md) relative to $m_z$ is $\pi/2-\operatorname{atan2}(b\omega,\kappa-I\omega^2)$. At $\omega=\omega_0$ it is zero, although the reaction [torque](torque.md) leads $m_z$ by $\pi/2$. A [phase](phase-waves.md) measured at the mirror is not automatically the [phase](phase-waves.md) of the applied [torque](torque.md).

A fixed-[amplitude](wave-amplitude.md) reference [torque](torque.md) $\tau_c\cos\omega t$ measures $|H_\tau|$ directly. The [Einstein-de Haas effect](einstein-de-haas-effect.md) instead contains an extra factor $\omega$ when $m_1$ stays fixed. Consequently its twist [amplitude](wave-amplitude.md) peaks exactly at $\omega_0$ in this model, whereas the fixed-[torque](torque.md) peak is at $\omega_0\sqrt{1-1/(2Q^2)}$ when $Q>1/\sqrt2$. To verify the first statement, divide the squared denominator of $A_{\rm EdH}$ by $\omega^2$: the quantity to minimize is $(\kappa/\omega-I\omega)^2+b^2$, minimized at $\omega_0$. Both response curves tend to zero at high [frequency](frequency.md); only the magnetomechanical curve also tends to zero at zero [frequency](frequency.md).

<a id="image-calibrated-forced-torsion-distinguish-the-mechanical-response-from-the-magnetic-drive"></a>
![](einstein-de-haas-calibrated-torsion-response.png)

**[Figure 13](#image-calibrated-forced-torsion-distinguish-the-mechanical-response-from-the-magnetic-drive). Calibrated forced torsion: distinguish the mechanical response from the magnetic drive**. Original calculated curves, not historical measurements or fitted data. A constant reference [torque](torque.md) and a constant-[amplitude](wave-amplitude.md) [magnetic dipole moment](magnetic-dipole-moment.md) share the same mechanical [transfer function](transfer-function.md). The lower plot uses each input's own cosine as its [phase](phase-waves.md) reference. Markers at $\omega_0=2\,\mathrm{rad/s}$ show equal twist [amplitudes](wave-amplitude.md) but different [phases](phase-waves.md).

For a fully stipulated example, choose $I=2.00\times10^{-10}\,\mathrm{kg\,m^2}$, $\kappa=8.00\times10^{-10}\,\mathrm{N\,m/rad}$, $b=8.00\times10^{-11}\,\mathrm{N\,m\,s/rad}$, $\gamma=-1.76\times10^{11}\,\mathrm{s^{-1}\,T^{-1}}$, and $m_1=1.76\times10^{-4}\,\mathrm{A\,m^2}$. These teaching inputs give $\omega_0=2.00\,\mathrm{rad/s}$, $Q=5.00$, reaction [torque](torque.md) [amplitude](wave-amplitude.md) $2.00\times10^{-15}\,\mathrm{N\,m}$ at $\omega_0$, and

$$
A_{\rm EdH}(\omega_0)=\frac{m_1}{|\gamma|b}=1.25\times10^{-5}\,\mathrm{rad}.
$$

An [optical lever](optical-lever.md) at distance $D=1.00\,\mathrm m$ gives small-displacement spot [amplitude](wave-amplitude.md) $x\simeq2DA=25.0\,\mu\mathrm m$; its full peak-to-peak width is $4DA=50.0\,\mu\mathrm m$. For a fast reversal from $+m_1$ to $-m_1$, the same inputs give $\Delta L_{\rm body}=-2.00\times10^{-15}\,\mathrm{kg\,m^2/s}$ and initial $\Delta\dot\theta=-1.00\times10^{-5}\,\mathrm{rad/s}$, provided the external angular [impulse](impulse.md) is negligible.

One independent mechanical calibration adds known [moment of inertia](moment-of-inertia.md) $\Delta I$, keeping $\kappa$ unchanged. If $T_a,T_b$ are the undamped [oscillation periods](period-of-an-oscillation.md) before and after adding it, then

$$
T_a^2=\frac{4\pi^2I}{\kappa},\qquad
T_b^2=\frac{4\pi^2(I+\Delta I)}{\kappa},\qquad
\kappa=\frac{4\pi^2\Delta I}{T_b^2-T_a^2}.
$$

For $\Delta I=I$ in the stipulated example, $T_a=\pi\,\mathrm s$ and $T_b=\sqrt2\pi\,\mathrm s$, recovering the chosen $I$ and $\kappa$. Real damped periods require a [damping](damping.md) correction: a free decay has angular envelope $e^{-bt/(2I)}$ and oscillation [angular frequency](angular-frequency.md) $\sqrt{\kappa/I-(b/(2I))^2}$. Measuring that decay determines $b/(2I)$. Calibrating the optical scale, mechanical response and change of [magnetic dipole moment](magnetic-dipole-moment.md) separately is what makes the inferred [gyromagnetic ratio](gyromagnetic-ratio.md) meaningful.

## ↑ Ancestors (7)

1. [Einstein-de Haas effect](einstein-de-haas-effect.md)
2. [Magnetic dipole moment](magnetic-dipole-moment.md)
3. [Magnetic vector potential](magnetic-vector-potential.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
