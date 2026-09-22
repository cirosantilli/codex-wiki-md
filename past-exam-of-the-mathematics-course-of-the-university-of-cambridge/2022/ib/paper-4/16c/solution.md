<h1 id="16c/solution">Solution</h1>

↑ **Parent:** [16C](../16c.md)

Irrotationality gives $\mathbf u_i=\nabla\phi_i$ and $\nabla^2\phi_i=0$. At $z=\zeta$, the exact kinematic conditions are

$$
\zeta_t+\phi_{ix}\zeta_x=\phi_{iz},
$$

and pressure continuity gives $p_1=p_2$. [Bernoulli equation](../../../../../bernoulli-equation.md) in each fluid is

$$
p_i=-\rho_i\left(\phi_{it}+\tfrac12|\nabla\phi_i|^2+gz\right)+C_i(t).
$$

Linearize at $z=0$ and write $\zeta=Ze^{i(kx-\omega t)}$. Decay at infinity gives

$$
\phi_1=A_1e^{-kz}e^{i(kx-\omega t)},
\qquad
\phi_2=A_2e^{kz}e^{i(kx-\omega t)}.
$$

The kinematic conditions give $-i\omega Z=-kA_1=kA_2$, while pressure continuity gives

$$
\rho_1(-i\omega A_1+gZ)=
ho_2(-i\omega A_2+gZ).
$$

Elimination yields

$$
\boxed{
\omega^2=gk\frac{\rho_2-\rho_1}{\rho_1+\rho_2},
\qquad F(r)=\frac{1-r}{1+r}}.
$$

Stable waves require the lower fluid to be denser, $\rho_2>\rho_1$; otherwise this is the [Rayleigh-Taylor instability](../../../../../rayleigh-taylor-instability.md).

## ↑ Ancestors (10)

1. [16C](../16c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
