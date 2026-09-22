<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [incompressibility](../../../../../../incompressible-flow.md), negligible [viscosity](../../../../../../dynamic-viscosity.md) and [surface tension](../../../../../../surface-tension.md), and an initially [irrotational flow](../../../../../../irrotational-flow.md). Take the undisturbed [free surface](../../../../../../free-surface.md) at $z=0$ and bed at $z=-H$. The [velocity potential](../../../../../../velocity-potential.md) $\varphi$ satisfies [Laplace equation](../../../../../../laplace-equation.md) and $\varphi_z(-H)=0$. For a [Fourier mode](../../../../../../fourier-mode.md), write

$$
\varphi=A\cosh[k(z+H)]e^{i(kx-\omega t)},\qquad \eta=\eta_a e^{i(kx-\omega t)},\qquad k>0.
$$

The linear [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) and linear [Bernoulli equation](../../../../../../bernoulli-equation.md) at the [free surface](../../../../../../free-surface.md) are $\eta_t=\varphi_z$ and $\varphi_t+g\eta=0$. Eliminating $A,\eta_a$ gives the [surface gravity wave](../../../../../../surface-gravity-wave.md) [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{\omega^2=gk\tanh(kH)}.
$$

The rightward [phase velocity](../../../../../../phase-velocity.md) and [group velocity](../../../../../../group-velocity.md) are

$$
c_p=\frac\omega k=\sqrt{\frac gk\tanh(kH)},\qquad c_g=\frac{d\omega}{dk}=\frac{c_p}{2}\left[1+\frac{2kH}{\sinh(2kH)}\right].
$$

The [phase velocity](../../../../../../phase-velocity.md) transports a crest; the [group velocity](../../../../../../group-velocity.md) transports a narrow-band envelope and its leading-order [energy](../../../../../../energy.md). For $kH\gg1$, $\omega\sim\sqrt{gk}$ and $c_g\sim c_p/2\sim\sqrt{g/k}/2$: deep-water [surface gravity waves](../../../../../../surface-gravity-wave.md) are dispersive. For $kH\ll1$, $\omega\sim k\sqrt{gH}$ and $c_g\sim c_p\sim\sqrt{gH}$, the nondispersive [shallow-water dispersion relation](../../../../../../shallow-water-dispersion-relation.md). The boundary [velocity](../../../../../../velocity.md) controls the excited amplitude; it does not change the linear [dispersion relation](../../../../../../dispersion-relation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
