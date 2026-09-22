<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

Let $u(t)$ be the signed air speed along the straw towards the bubble. [Conservation of mass in a pipe](../../../../../conservation-of-mass-in-a-pipe.md) for the incompressible plug flow gives

$$
\pi\varepsilon^2u=\frac d{dt}\left(\frac{4\pi a^3}{3}\right),
\qquad
u=\frac{4a^2\dot a}{\varepsilon^2}.
$$

The unsteady [Bernoulli equation](../../../../../bernoulli-equation.md) along the straw, whose open end is at atmospheric pressure, gives

$$
p_{\rm in}-p_{\rm atm}=-\rho L\dot u=\frac{2\gamma}{a}
$$

by the [Young–Laplace equation](../../../../../young-laplace-equation.md). Substitution yields

$$
a^3\ddot a+2a^2\dot a^2=-\frac{\gamma\varepsilon^2}{2\rho L}=-C.
$$

Set $w=a^2\dot a$. Since $a\dot w=-C$, the [chain rule](../../../../../chain-rule.md) gives $w\,dw/da=-Ca$. The initial condition $\dot a(0)=0$ implies

$$
a^4\dot a^2=C(a_0^2-a^2),
\qquad
a^2\dot a=-\sqrt{C(a_0^2-a^2)}.
$$

Writing $a=a_0\sin\theta$ and integrating gives the implicit solution

$$
t=\frac{a_0^2}{2\sqrt C}\left[\frac\pi2-\theta+\sin\theta\cos\theta\right],
\qquad \theta=\sin^{-1}(a/a_0).
$$

At disappearance $a=0$ and $\theta=0$, so

$$
\boxed{t_*=\frac{\pi a_0^2}{2\varepsilon}\left(\frac{\rho L}{2\gamma}\right)^{1/2}.}
$$

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
