<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The displayed oscillator expansion and the displayed [action](../../../../action.md) require two separate corrections to describe one conventional positive-energy theory.** First compute what the oscillator algebra literally implies. Assume the two oscillator species commute with each other and annihilate the [vacuum](../../../../vacuum.md). Same-charge contractions vanish, so

$$
\boxed{\langle T\phi(x)\phi(y)\rangle_0
=\langle T\phi^*(x)\phi^*(y)\rangle_0=0.}
$$

For the two mixed contractions the printed phases give the same kernel, with $z=x-y$:

$$
\begin{aligned}
C_{\mathrm{lit}}(z)
&=\theta(z^0)\int\frac{d^3p}{(2\pi)^3\,2E_{\mathbf p}}e^{+ip\cdot z}
+\theta(-z^0)\int\frac{d^3p}{(2\pi)^3\,2E_{\mathbf p}}e^{-ip\cdot z}\\
&=\int\frac{d^4p}{(2\pi)^4}\frac{-i\,e^{-ip\cdot z}}{p^2-m^2-i0}.
\end{aligned}
$$

Thus $\langle T\phi(x)\phi^*(y)\rangle_0=\langle T\phi^*(x)\phi(y)\rangle_0=C_{\mathrm{lit}}(z)$. In $D$ dimensions replace $d^3p$ and $d^4p$ by $d^{D-1}p$ and $d^Dp$; the source's explicit three-dimensional spatial measure is the $D=4$ specialization. The covariant integral is manifestly [Lorentz invariant](../../../../lorentz-invariance.md). With

$$
D_F(z)=\int\frac{d^Dp}{(2\pi)^D}\frac{i\,e^{-ip\cdot z}}{p^2-m^2+i0},
$$

we have $C_{\mathrm{lit}}(z)=D_F(z)^*$. This [reversed-frequency scalar contraction](../../../../reversed-frequency-scalar-contraction.md) has the opposite pole prescription to the usual positive-energy [Feynman propagator](../../../../feynman-propagator.md). For a single zero-[momentum](../../../../momentum-split.md) mode at positive time separation, the printed contraction is $e^{+imt}/(2m)$, while $D_F$ is $e^{-imt}/(2m)$: this is a concrete phase counterexample, rather than an immaterial change of integration variable.

There is also a [normalization of a complex scalar propagator](../../../../normalization-of-a-complex-scalar-propagator.md) conflict independent of those phases. The displayed [Lagrangian density](../../../../lagrangian-density.md) gives the [canonical momentum](../../../../canonical-momentum.md) $\pi_\phi=\dot\phi^*/2$. Substituting the printed modes yields

$$
[\phi(t,\mathbf x),\pi_\phi(t,\mathbf y)]
=-\frac i2\delta^{(3)}(\mathbf x-\mathbf y),
$$

instead of the canonical $+i\delta^{(3)}$. Reversing the mode phases repairs the sign but leaves $+i\delta^{(3)}/2$, so it does not repair the normalization. The [complex scalar field](../../../../complex-scalar-field.md) convention with unit mixed propagator normally has no $1/2$ in its quadratic action.[§2.5, equations (2.67)–(2.73): complex-field kinetic normalization and canonical commutators](../../../../quantum-field-theory-by-david-tong.md)

To retain the actual action in the paper, use $\phi=\phi_1+i\phi_2$ with canonically normalized real components, or equivalently replace its mode expansion by

$$
\phi(x)=\int\frac{d^{D-1}p}{(2\pi)^{D-1}\sqrt{E_{\mathbf p}}}
\left(a_{\mathbf p}e^{-ip\cdot x}+b_{\mathbf p}^\dagger e^{ip\cdot x}\right).
$$

The corresponding [path integral](../../../../path-integral.md) with the usual [Feynman i-epsilon prescription](../../../../feynman-i-epsilon-prescription.md) has

$$
\boxed{C(x,y)\equiv\langle T\phi(x)\phi^*(y)\rangle_0
=\langle T\phi^*(x)\phi(y)\rangle_0=2D_F(x-y),}
$$

with the two same-charge propagators still zero. This action-consistent kernel is used in [b](../b.md) and [c](../c.md). Keeping conventional unit modes instead would require removing the quadratic factors $1/2$ from the action as well as reversing the phases. Those are distinct theories unless the field and its coupling are rescaled together.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
