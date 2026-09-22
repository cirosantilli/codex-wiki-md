<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $x(0)=0$. Integrating the [velocity](../../../../../../velocity.md) solution gives

$$
x(t)=v_0\tau(1-e^{-t/\tau})+\frac1\zeta\int_0^t[1-e^{-(t-s)/\tau}]F(s)\,ds.
$$

The initial/noise cross term vanishes under the independence assumption. Evaluating the remaining integral yields the general [integrated Ornstein-Uhlenbeck displacement](../../../../../../integrated-ornstein-uhlenbeck-displacement.md)

$$
\langle x(t)^2\rangle=\langle v_0^2\rangle\tau^2(1-e^{-t/\tau})^2+\frac A{\zeta^2}\left[t-2\tau(1-e^{-t/\tau})+\frac\tau2(1-e^{-2t/\tau})\right].
$$

Use the thermal initial [velocity](../../../../../../velocity.md) and the [fluctuation-dissipation relation for a Langevin particle](../../../../../../fluctuation-dissipation-relation-for-a-langevin-particle.md). With [diffusion coefficient](../../../../../../diffusion-coefficient.md) $D=k_BT/\zeta$, this simplifies to

$$
\boxed{\langle x(t)^2\rangle=2D\left[t-\tau(1-e^{-t/\tau})\right].}
$$

For $t\ll\tau$, expansion gives $\langle x^2\rangle=(k_BT/m)t^2+O(t^3)$: displacement is initially $v_0t$, so the particle is **ballistic**. For $t\gg\tau$, $\langle x^2\rangle=2Dt-2D\tau+o(1)$, hence the leading behavior is **one-dimensional [diffusion](../../../../../../diffusion.md) with $D=k_BT/(6\pi\mu a)$**.

The ballistic conclusion depends on the initial state. For a particle prepared exactly at rest, $v_0=0$, the first expression gives $\langle x^2\rangle=A t^3/(3m^2)+O(t^4)$ at very short times. A thermal initial [velocity](../../../../../../velocity.md), or a nonzero initial [velocity](../../../../../../velocity.md) variance, is required for the stated $t^2$ mean-square law. It should not be replaced silently by a zero-[velocity](../../../../../../velocity.md) initial condition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
