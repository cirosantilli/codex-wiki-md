<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The linear [dispersion relation](../../../../../../dispersion-relation.md) for a mode $e^{i(kx-\omega t)}$ is $5\omega^2=k^4+4$. The proposed modes share [phase velocity](../../../../../../phase-velocity.md) $c$, so $5c^2k_j^2=k_j^4+4$. A [quadratic wave interaction](../../../../../../quadratic-wave-interaction.md) generates the second harmonic and the difference harmonic. With only two positive [wavenumbers](../../../../../../wavenumber.md), [phase matching for a quadratic wave interaction](../../../../../../phase-matching-for-a-quadratic-wave-interaction.md) requires $k_2=2k_1$. Equating their phase velocities gives

$$
k_1^2+\frac4{k_1^2}=4k_1^2+\frac1{k_1^2},
$$

and therefore

$$
\boxed{k_1=1,\qquad k_2=2,\qquad c=1.}
$$

This is a [two-to-one resonance of dispersive waves](../../../../../../two-to-one-resonance-of-dispersive-waves.md). Its amplitude changes accumulate on $t=O(\epsilon^{-1})$. Choose the [slow time](../../../../../../slow-time.md) $T=\epsilon t/5$; this harmless constant rescaling makes the later amplitude formulas simple. With $\xi=x-t$, the leading real field is $A_0e^{i\xi}+B_0e^{2i\xi}+\overline A_0e^{-i\xi}+\overline B_0e^{-2i\xi}$.

For the fundamental, the order-$\epsilon$ cross derivative in $5\psi_{tt}$ is $-2i(A_0)_T e^{i\xi}$, while the fundamental coefficient in $\psi_0\psi_{0x}$ is $i\overline A_0B_0$. For the second harmonic the corresponding terms are $-4i(B_0)_T e^{2i\xi}$ and $iA_0^2$. The [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md) removes the resonant forcing and gives

$$
\boxed{(A_0)_T=-\frac12\overline A_0B_0,\qquad (B_0)_T=-\frac14A_0^2.}
$$

The nonresonant third and fourth harmonics enter the correction. They do not change these leading [amplitude equations](../../../../../../amplitude-equation.md).

Write $A_0=Re^{i\theta}$, $B_0=Pe^{i\phi}$ and $\delta=\phi-2\theta$. Taking real and imaginary parts gives the [explosive two-to-one amplitude system](../../../../../../explosive-two-to-one-amplitude-system.md) in polar form:

$$
\boxed{R_T=-\frac{RP}2\cos\delta,\qquad \theta_T=-\frac P2\sin\delta,\qquad P_T=-\frac{R^2}4\cos\delta,\qquad \phi_T=\frac{R^2}{4P}\sin\delta.}
$$

The polar phases are used where their corresponding amplitudes are nonzero. These equations imply

$$
(R^2-2P^2)_T=0,\qquad (R^2P\sin\delta)_T=0.
$$

For the second identity, differentiate using $\delta_T=(R^2/(4P)+P)\sin\delta$: the terms proportional to $\sin\delta\cos\delta$ cancel. Therefore

$$
R^2\theta_T=-\frac12R^2P\sin\delta,\qquad P^2\phi_T=\frac14R^2P\sin\delta
$$

are [first integrals](../../../../../../first-integral.md), and in particular

$$
\boxed{(R^2\theta_T)_T=0,\qquad(P^2\phi_T)_T=0.}
$$

For constant phases with $\phi=2\theta+\pi$, these real equations reduce to $R_T=RP/2$ and $P_T=R^2/4$. The initial data give $R^2-2P^2=8$, so the [Riccati equation](../../../../../../riccati-equation.md) for $P$ is $2P_T=P^2+4$. Integrating and using $P(0)=2$ gives

$$
\boxed{P(T)=2\tan(T+\pi/4),\qquad R(T)=2\sqrt2\sec(T+\pi/4),\qquad 0\leq T<\pi/4.}
$$

The [tangent](../../../../../../tangent.md) and [secant function](../../../../../../secant-trigonometry.md) have a pole at $T=\pi/4$, corresponding to $t=5\pi/(4\epsilon)$. Both modes grow through their locked resonant interaction. This is formal [finite-time blowup](../../../../../../finite-time-blowup.md) of the reduced [amplitude equations](../../../../../../amplitude-equation.md); the [weakly nonlinear expansion](../../../../../../weakly-nonlinear-expansion.md) loses validity as the amplitudes become large, so it cannot establish a singularity of the full partial differential equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
