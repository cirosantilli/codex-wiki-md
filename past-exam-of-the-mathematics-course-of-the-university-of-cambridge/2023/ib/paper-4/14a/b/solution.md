<h1 id="14a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The causal [Green function](../../../../../../green-s-function.md) for the heat operator is

$$
G(x,t;\xi,\tau)=H(t-\tau)
\frac1{\sqrt{4\pi D(t-\tau)}}
\exp\left[-\frac{(x-\xi)^2}{4D(t-\tau)}\right],
$$

where $H$ is the [Heaviside step function](../../../../../../heaviside-step-function.md). It vanishes for $t<\tau$, satisfies the homogeneous heat equation away from the source, and approaches $\delta(x-\xi)$ as $t\downarrow\tau$. Superposing the responses to all infinitesimal sources gives [Duhamel principle](../../../../../../duhamel-s-principle.md):

$$
\boxed{
\theta_f(x,t)=\int_0^t\int_{-\infty}^{\infty}
\frac{\exp\left[-\dfrac{(x-\xi)^2}{4D(t-\tau)}\right]}
{\sqrt{4\pi D(t-\tau)}}
f(\xi,\tau)\,d\xi\,d\tau}.
$$

The lower limit and causality give the required homogeneous initial data.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14A](../../14a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
