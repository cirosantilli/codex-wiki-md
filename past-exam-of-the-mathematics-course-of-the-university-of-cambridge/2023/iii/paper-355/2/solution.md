<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In the small-slope approximation the [worm-like chain](../../../../../worm-like-chain.md) bending energy is

$$
E[h]=\frac A2\int_0^L h_{xx}^2\,dx.
$$

The clamped end obeys $h(0)=h_x(0)=0$, while a force-free and torque-free tip has the natural conditions $h_{xx}(L)=h_{xxx}(L)=0$. A static transverse tip force $f$ produces the cantilever compliance $h(L)/f=L^3/(3A)$. The [equipartition theorem](../../../../../equipartition-theorem.md), or equivalently the static fluctuation--response relation, therefore gives the exact tip variance

$$
\boxed{\langle h(L)^2\rangle=\frac{k_BT L^3}{3A}
=\frac{L^3}{3L_p}.}
$$

For the dynamics, [resistive-force theory](../../../../../resistive-force-theory.md) gives the transverse drag per length

$$
\zeta_\perp\simeq\frac{4\pi\mu}{\log(L/a)+1/2}
$$

at logarithmic accuracy and the stochastic beam equation

$$
\zeta_\perp\partial_t h=-A\partial_x^4h+f_T.
$$

Let $\phi_n$ be clamped--free bending modes with $q_nL=\alpha_n$, where

$$
\cos\alpha_n\cosh\alpha_n=-1,
\qquad \alpha_1\simeq1.875.
$$

Writing $N_n=\int_0^L\phi_n^2dx$, independent thermally driven modes give

$$
\boxed{\langle h(L,t)h(L,0)\rangle
=\sum_{n=1}^\infty
\frac{k_BT\phi_n(L)^2}{Aq_n^4N_n}
e^{-|t|/\tau_n},
\qquad
\tau_n=\frac{\zeta_\perp}{Aq_n^4}.}
$$

The first mode contains almost all of the tip variance, so

$$
\langle h(L,t)h(L,0)\rangle
\simeq\frac{k_BT L^3}{3A}e^{-|t|/\tau_1},
\qquad
\tau_1=\frac{\zeta_\perp L^4}{A\alpha_1^4}.
$$

For a microtubule, $A=k_BT L_p$. With $L=10\,\mu\mathrm m$ and $L_p=3\,\mathrm{mm}$,

$$
\boxed{\sqrt{\langle h(L)^2\rangle}
=\sqrt{\frac{L^3}{3L_p}}
\simeq0.33\,\mu\mathrm m.}
$$

Taking water at room temperature and $a=0.5\,\mu\mathrm m$ gives $\zeta_\perp\simeq3.6\times10^{-3}\,\mathrm{Pa\,s}$ and

$$
\boxed{\tau_1\simeq0.24\,\mathrm s,}
$$

with an order-one uncertainty from the logarithmic slender-body drag approximation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 355](../../paper-355-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
