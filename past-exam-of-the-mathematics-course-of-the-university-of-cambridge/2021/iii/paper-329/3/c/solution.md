<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the torus frame the two planes translate with velocity $U\mathbf e_x$. Away from the $O(a)$ neighborhood of the torus, the depth-averaged [Hele-Shaw flow](../../../../../../hele-shaw-flow.md) between planes separated by $2a$ is

$$
\overline{\mathbf u}
=U\mathbf e_x-\frac{a^2}{3\mu}\nabla p,
\qquad
\nabla^2p=0.
$$

Negligible leakage imposes $\overline u_r=0$ at $r=R$. The harmonic pressure that decays at infinity in the exterior and the regular harmonic pressure in the interior are therefore

$$
\boxed{
p_{>}(r,\theta)
=-\frac{3\mu UR^2}{a^2r}\cos\theta,
\qquad
p_{<}(r,\theta)
=\frac{3\mu U}{a^2}r\cos\theta},
$$

up to a common constant. The interior velocity is zero, while the exterior flow is the uniform stream diverted around a circular obstacle. In plan view the inside has high pressure on the $+x$ side and low pressure on the $-x$ side; the immediately adjacent exterior has the opposite signs, producing the pressure jump across the torus.

The jump at $r=R$ is

$$
p_<-p_>=\frac{6\mu UR}{a^2}\cos\theta.
$$

Integrating it over the projected vertical area $2aR\,d\theta$ gives the global pressure resistance

$$
\boxed{F_x\sim\frac{12\pi\mu UR^2}{a}}.
$$

There are two narrow gaps, so their local resistance is twice the one-plane result from part b:

$$
F_{\rm gap}\sim12\pi^2\mu UR\varepsilon^{-1/2}.
$$

Consequently the local gap resistance dominates when $a\ll R\ll a\varepsilon^{-1/2}$, whereas the global Hele–Shaw pressure resistance dominates when

$$
a\varepsilon^{-1/2}\ll R\ll a\varepsilon^{-5/2}.
$$

To interpret the upper bound, the pressure jump has scale $\Delta p\sim\mu UR/a^2$. Each narrow gap has thickness $a\varepsilon$ and streamwise lubrication length $a\sqrt\varepsilon$. Its pressure-driven leakage flux per unit centreline length therefore scales as

$$
q_{\rm leak}
\sim\frac{(a\varepsilon)^3}{\mu a\sqrt\varepsilon}\Delta p
\sim UR\varepsilon^{5/2}.
$$

The blocked Hele–Shaw flux has scale $Ua$. Leakage is negligible precisely when $UR\varepsilon^{5/2}\ll Ua$, or

$$
\boxed{R\ll a\varepsilon^{-5/2}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
