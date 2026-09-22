<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose the relative phases of the two [energy eigenstates](../../../../energy-eigenstate.md) so that $d=\langle\psi_2|\widehat D_0|\psi_1\rangle$ is real and nonnegative. Define the resonant [Rabi angular frequency](../../../../rabi-angular-frequency.md) $\Omega=d/\hbar$, the [Rabi detuning](../../../../rabi-detuning.md) $\delta=\omega_0-\omega$, and $\Sigma=\omega_0+\omega$. Substitution into the [Schrödinger equation](../../../../schrodinger-equation.md), followed by projection onto the two [eigenstates](../../../../eigenstate.md), gives the exact [interaction picture](../../../../interaction-picture.md) equations

$$
i\dot c_1=\frac{\Omega}{2}(e^{-i\delta t}+e^{-i\Sigma t})c_2,\qquad
i\dot c_2=\frac{\Omega}{2}(e^{i\delta t}+e^{i\Sigma t})c_1.
$$

Keep both [probability amplitudes](../../../../probability-amplitude.md) dynamical: replacing $c_1$ by one would incorrectly impose weak excitation and miss complete population transfer.

For $|\delta|,\Omega\ll\omega_0$, apply the [rotating-wave approximation](../../../../rotating-wave-approximation.md) to discard the rapidly oscillating terms at $\Sigma$. Differentiating the second remaining equation and using the first gives

$$
\ddot c_2-i\delta\dot c_2+\frac{\Omega^2}{4}c_2=0.
$$

The [initial conditions](../../../../initial-condition.md) are $c_2(0)=0$ and $\dot c_2(0)=-i\Omega/2$. With $\Omega_R=\sqrt{\Omega^2+\delta^2}$, their solution is

$$
c_2(t)=-i\frac{\Omega}{\Omega_R}e^{i\delta t/2}\sin\frac{\Omega_Rt}{2},\qquad
c_1(t)=e^{-i\delta t/2}\left(\cos\frac{\Omega_Rt}{2}+i\frac{\delta}{\Omega_R}\sin\frac{\Omega_Rt}{2}\right).
$$

Consequently,

$$
\boxed{|c_2(t)|^2=U\sin^2(\alpha t),\qquad
U=\frac{\Omega^2}{\Omega^2+\delta^2},\qquad
\alpha=\tfrac12\sqrt{\Omega^2+\delta^2}.}
$$

This result permits order-one excitation, including full population transfer on [resonance](../../../../resonance.md), even though the drive is small compared with the optical [angular frequency](../../../../angular-frequency.md).

For an average from switch-on to time $\tau$, integrate the squared sine:

$$
\boxed{\overline P_2(\tau)=\frac1\tau\int_0^\tau|c_2(t)|^2dt
=\frac U2\left[1-\frac{\sin(\Omega_R\tau)}{\Omega_R\tau}\right],\qquad
\lim_{\tau\to\infty}\overline P_2=\frac U2.}
$$

On [resonance](../../../../resonance.md) this limiting average is $1/2$, although the instantaneous [probability](../../../../probability.md) repeatedly reaches one. The zero-coupling, zero-[Rabi detuning](../../../../rabi-detuning.md) case is understood separately as $P_2=0$.

**Near [resonance](../../../../resonance.md) alone does not make this an exact result for arbitrarily strong driving.** The stated sinusoidal [Hamiltonian](../../../../hamiltonian.md) also needs the [rotating-wave approximation](../../../../rotating-wave-approximation.md). A concrete counterexample is $\omega=\omega_0$ and $\Omega=\omega_0$: the exact equations give $P_2(t)=\Omega^2t^2+O(t^4)$ at switch-on, while the claimed rotating-wave sinusoid gives $\Omega^2t^2/4+O(t^4)$. Thus “without assuming weak radiation” can mean without assuming small excitation, but cannot remove the drive-to-carrier scale separation. The infinite-time average above belongs to the rotating-wave model; omitted corrections can accumulate over sufficiently long times.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
