<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For zero [damping](../../../../damping.md) the conserved [mechanical energy](../../../../mechanical-energy.md) is

$$
\boxed{H=\tfrac12\dot x^2+V(x)=\tfrac12v^2,\qquad V(x)=\tfrac12x^2-\tfrac\gamma4x^4.}
$$

For $\gamma<0$, the potential grows to infinity in both directions, so every nonstationary finite-energy trajectory is trapped between two [turning points](../../../../turning-point.md) and is periodic; the zero-energy solution is stationary. The case $\gamma=0$ is the [harmonic oscillator](../../../../simple-harmonic-motion.md). The negative-$\gamma$ comparison extends the parameter range initially stated in the source.

For $\gamma>0$, the origin lies in a local potential well, with barriers at $x=\pm\gamma^{-1/2}$ of height $1/(4\gamma)$. A trajectory launched from the origin oscillates precisely when its initial energy is below that barrier:

$$
\boxed{|v|<\frac1{\sqrt{2\gamma}}.}
$$

At equality the trajectory approaches a barrier [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) asymptotically, rather than being periodic; for example the positive branch is $x=\gamma^{-1/2}\tanh(t/\sqrt2)$. Above the barrier the trajectory escapes the well. The source's inequality without the absolute value tacitly takes $v\geq0$; for signed initial velocity the energy criterion requires $|v|$.

Next set $\beta=\gamma=0$ and assume $\alpha>0$. The energy $H=(\dot x^2+x^2)/2$ satisfies $\dot H=-\alpha x^2\dot x^2\leq0$. This bounds the complete trajectory. The zero-dissipation set is the union of $x=0$ and $\dot x=0$, and its only invariant trajectory is the origin: a nonzero point on either axis immediately leaves it under the differential equation. The [LaSalle invariance principle](../../../../lasalle-s-invariance-principle.md) therefore gives $\boxed{x(t)\to0,\quad\dot x(t)\to0}$. If $\alpha=0$ as well, [damping](../../../../damping.md) is absent and that conclusion fails for nonzero $v$; the positive order-one [damping](../../../../damping.md) assumption is essential.

For the weakly nonlinear periodic motion, write $\gamma=\alpha\kappa$, set $\tau=\omega t$, $\omega=1+\alpha\omega_1+\cdots$, and expand $x=A\cos\tau+\alpha x_1+\cdots$. The first correction obeys

$$
x_1''+x_1=A(A^2/4-\beta)\sin\tau+
(2\omega_1A+3\kappa A^3/4)\cos\tau
+\frac{A^3}4\sin3\tau+\frac{\kappa A^3}4\cos3\tau.
$$

Resonant forcing at the [fundamental frequency](../../../../fundamental-frequency.md) would generate [secular terms](../../../../secular-term.md). Eliminating both coefficients yields

$$
\boxed{A=2\sqrt\beta,\qquad\omega_1=-\frac{3\kappa A^2}{8},\qquad
\omega=1-\frac32\gamma\beta+O(\alpha^2).}
$$

Consequently the maximum displacement is $\boxed{2\sqrt\beta+O(\alpha)}$ for fixed positive $\beta$. A possible third-harmonic correction is $x_1=-A^3\sin3\tau/32-\kappa A^3\cos3\tau/32$, up to homogeneous [amplitude](../../../../wave-amplitude.md) and [phase](../../../../phase-waves.md) choices. The leading [amplitude](../../../../wave-amplitude.md) also balances averaged [damping](../../../../damping.md): its slow evolution is $\dot A=\alpha A(\beta/2-A^2/8)$, whose nonzero fixed point is attracting. The case $\beta=0$ is a degenerate zero-[amplitude](../../../../wave-amplitude.md) limit, rather than a nonzero [limit cycle](../../../../limit-cycle.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the differential equations and applications course of the University of Oxford](../../../split.md)
5. [Differential equations and applications course of the University of Oxford](../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
