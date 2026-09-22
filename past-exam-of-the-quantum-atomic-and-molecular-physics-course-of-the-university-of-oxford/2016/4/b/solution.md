<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At first order in [time-dependent perturbation theory](../../../../time-dependent-perturbation-theory.md) set $c_1\simeq1$ and use the [parity](../../../../parity.md) result $V_{22}=0$. Decomposing the cosine into its two exponentials gives

$$
c_2(t)=-\frac{i\Omega}{2}\int_0^t
[e^{i(\omega_0-\omega)t'}+e^{i(\omega_0+\omega)t'}]dt'.
$$

Both exponentials contribute to the exact first-order result:

$$
\boxed{c_2(t)=-\frac\Omega2\left[
\frac{e^{i(\omega_0-\omega)t}-1}{\omega_0-\omega}
+\frac{e^{i(\omega_0+\omega)t}-1}{\omega_0+\omega}\right].}
$$

Each apparent zero denominator has a continuous limit. In particular the near-resonant fraction tends to $it$ as $\omega\to\omega_0$, while the counter-rotating fraction remains bounded on the optical timescale. One may equivalently write the expression as

$$
c_2(t)=-\frac{i\Omega t}{2}\sum_{\epsilon=\pm1}
 e^{i(\omega_0+\epsilon\omega)t/2}
\operatorname{sinc}[(\omega_0+\epsilon\omega)t/2],
\qquad\operatorname{sinc}u=\frac{\sin u}{u}.
$$

This form makes $c_2(0)=0$ explicit and avoids cancellation at resonance. At extremely short time both [sinc functions](../../../../sinc-function.md) tend to one, so $c_2\simeq-i\Omega t$, agreeing with the initial derivative of the original cosine-driven equation. No [rotating-wave approximation](../../../../rotating-wave-approximation.md) has yet been made. The separate assumption of weak excitation remains necessary: the first-order expression must not be extended until it predicts [probabilities](../../../../probability.md) comparable to or larger than one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum, atomic and molecular physics course of the University of Oxford](../../../split.md)
5. [Quantum, atomic and molecular physics course of the University of Oxford](../../../../quantum-atomic-and-molecular-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
