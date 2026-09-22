<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\mathcal T=\beta\hbar>0$, the interval of [imaginary time](../../../../imaginary-time.md), and assume $m,\omega>0$. For a [variation](../../../../variation.md) $x_0+\epsilon\eta$ with $\eta(0)=\eta(\mathcal T)=0$, the [first variation](../../../../first-variation.md) of the [Euclidean action](../../../../euclidean-action.md) is

$$
\delta S=m\int_0^{\mathcal T}(\dot x_0\dot\eta+\omega^2x_0\eta)\,d\tau
=m[\dot x_0\eta]_0^{\mathcal T}
+m\int_0^{\mathcal T}(-\ddot x_0+\omega^2x_0)\eta\,d\tau.
$$

The [boundary term](../../../../boundary-term.md) vanishes. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore gives the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md)

$$
\boxed{\ddot x_0=\omega^2x_0.}
$$

Its sign differs from the real-[time](../../../../time-in-physics.md) [harmonic oscillator equation](../../../../simple-harmonic-motion.md) because the [Euclidean action](../../../../euclidean-action.md) contains positive [kinetic energy](../../../../kinetic-energy.md) and positive [potential energy](../../../../potential-energy.md). The general solution is $A\cosh(\omega\tau)+B\sinh(\omega\tau)$. Applying the two endpoint conditions gives $A=x$ and $B=-x\tanh(\omega\mathcal T/2)$. Equivalently, the [equal-endpoint Euclidean oscillator path](../../../../equal-endpoint-euclidean-oscillator-path.md) is

$$
\boxed{x_0(\tau)=x\frac{\cosh[\omega(\tau-\mathcal T/2)]}{\cosh(\omega\mathcal T/2)}.}
$$

This form displays reflection about the midpoint and satisfies both endpoints immediately. On this path,

$$
\frac d{d\tau}(x_0\dot x_0)=\dot x_0^2+x_0\ddot x_0
=\dot x_0^2+\omega^2x_0^2.
$$

Thus the [Euclidean action](../../../../euclidean-action.md) reduces to a [boundary term](../../../../boundary-term.md). Since $\dot x_0(\mathcal T)=\omega x\tanh(\omega\mathcal T/2)$ and $\dot x_0(0)=-\omega x\tanh(\omega\mathcal T/2)$,

$$
S[x_0]=\frac m2[x_0\dot x_0]_0^{\mathcal T}
=\boxed{m\omega x^2\tanh\!\left(\frac{\beta\hbar\omega}{2}\right).}
$$

The positive [quadratic form](../../../../quadratic-form-split.md) $m\int_0^{\mathcal T}(\dot\eta^2+\omega^2\eta^2)\,d\tau$ is the [second variation](../../../../second-variation.md), so this stationary path is the unique minimum, rather than merely an arbitrary [stationary point](../../../../stationary-point.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
