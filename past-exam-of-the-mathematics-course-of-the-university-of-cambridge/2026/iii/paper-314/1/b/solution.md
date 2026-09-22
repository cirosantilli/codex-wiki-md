<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $Df/Dt=0$, the density ansatz has

$$
\frac1\rho\frac{D\rho}{Dt}=\frac{\dot\rho_0}{\rho_0}.
$$

The velocity divergence is

$$
\nabla\mathbin\cdot\mathbf u=A+B+C
=\frac d{dt}\log(abc).
$$

The [mass conservation](../../../../../../mass-conservation.md) equation therefore gives

$$
\boxed{\rho_0\propto(abc)^{-1}}.
$$

Similarly,

$$
\frac1p\frac{Dp}{Dt}
=\frac{\dot\rho_0}{\rho_0}+\frac{\dot T}{T}
=-\gamma\nabla\mathbin\cdot\mathbf u,
$$

and hence

$$
\boxed{T\propto(abc)^{-(\gamma-1)}}.
$$

The $x$ component of the material acceleration is

$$
\frac{Du_x}{Dt}=(\dot A+A^2)x=\frac{\ddot a}{a}x.
$$

Because $d\widehat p/df=\widehat\rho$,

$$
-\frac1\rho\partial_xp
=-\frac1{\rho_0\widehat\rho}
\rho_0T\widehat\rho\left(-\frac{2x}{a^2}\right)
=\frac{2Tx}{a^2}.
$$

Combining this with $-\partial_x\Phi=-\Omega^2x$ gives

$$
\boxed{\ddot a+\Omega^2a=\frac{2T}{a}}.
$$

The $y$ and $z$ components give the analogous equations for $b$ and $c$. Finally, $\widehat p(0)=0$ makes $p=0$ on the material free surface, so both dynamic and [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) requirements are satisfied.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
