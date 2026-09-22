<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

For an [inviscid flow](../../../../../inviscid-flow.md) that is an [incompressible flow](../../../../../incompressible-flow.md) and an [irrotational flow](../../../../../irrotational-flow.md), write $\mathbf u=\nabla\phi$. The [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md), without gravity, integrate spatially to the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md)

$$
\boxed{\frac{\partial\phi}{\partial t}+\frac12|\nabla\phi|^2+\frac p\rho=C(t).}
$$

A time-dependent addition to $\phi$ can absorb $C(t)$.

In the ideal uniform tube-plug model, let $u(t)$ be the axial speed toward the outlet. Incompressibility and fixed cross-section make the speed the same at both ends. With $\phi=u(t)x$, the kinetic terms cancel when the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md) is subtracted between entrance and exit, giving

$$
L\dot u=\frac{p_{\rm in}-p_{\rm out}}\rho=\frac{2\gamma}{\rho R}.
$$

Conservation of volume in the spherical balloon gives $4\pi R^2\dot R=-\pi a^2u$, or $u=-4R^2\dot R/a^2$. Differentiating and eliminating $u$ yields

$$
-\frac{4L}{a^2}(R^2\ddot R+2R\dot R^2)=\frac{2\gamma}{\rho R},\qquad \boxed{R^3\ddot R+2R^2\dot R^2=-K},\quad K=\frac{\gamma a^2}{2\rho L}.
$$

This is the [constant-tension balloon discharge](../../../../../constant-tension-balloon-discharge.md) equation; entrance losses and a reservoir-to-tube kinetic-head correction are excluded by this ideal plug model.

Multiplication by $2R\dot R$ turns the equation into

$$
\frac d{dt}(R^4\dot R^2)=-K\frac d{dt}(R^2),\qquad R^4\dot R^2+KR^2=C.
$$

The printed time formula additionally assumes the water is initially at rest, $\dot R(0)=0$, although only $R_0$ is explicitly specified in the question. Under that assumption $C=KR_0^2$. On the shrinking branch,

$$
\dot R=-\frac{\sqrt K\sqrt{R_0^2-R^2}}{R^2},\qquad t=\frac1{\sqrt K}\int_R^{R_0}\frac{r^2}{\sqrt{R_0^2-r^2}}\,dr.
$$

Set $r=R_0\sin\vartheta$ and $\theta=\arcsin(R/R_0)$. The [integral](../../../../../integral.md) becomes $R_0^2K^{-1/2}\int_\theta^{\pi/2}\sin^2\vartheta\,d\vartheta$, hence

$$
\boxed{t=R_0^2\sqrt{\frac{2\rho L}{\gamma a^2}}\left(\frac\pi4-\frac\theta2+\frac{\sin2\theta}{4}\right).}
$$

Putting $R=0$, or $\theta=0$, gives the ideal **emptying time**

$$
\boxed{t_{\rm empty}=\frac{\pi R_0^2}{4}\sqrt{\frac{2\rho L}{\gamma a^2}}.}
$$

For an independently prescribed initial rate $v_0=\dot R(0)$, the [first integral](../../../../../first-integral.md) instead has $C=KR_0^2+R_0^4v_0^2$, so radius alone does not determine that emptying time. This explicitly identifies the extra initial datum needed for the displayed answer.

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
