<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The nonzero [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are paired by reflection:

$$
x_*=\pm\sqrt{3(1-c/d)},\qquad y_*=0,\qquad z_*=(c/d)x_*,\qquad 0<c<d.
$$

At either [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md), the derivative of the second equation with respect to $x$ is $-1+x_*^2=2-3c/d$. The [characteristic polynomial](../../../../../../characteristic-polynomial.md) becomes

$$
p_*(m)=m^3+(2-d/2)m^2+(3c/d-d-2)m+(d-c).
$$

Its constant term is nonzero away from the [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md), so there is no further steady local bifurcation. At a [Hopf bifurcation](../../../../../../hopf-bifurcation.md) the condition $A_1A_2=A_3$ gives

$$
\boxed{c_H^*(d)={d(8+4d-d^2)\over12-d},\qquad0<d<1,\qquad
\omega^2={2d(1-d)\over12-d}.}
$$

Indeed $\tau=2-d/2$ and $\tau\omega^2=d-c>0$ require $d<4$; within this range $\omega^2>0$ is equivalent to $d<1$. The apparent singularity at $d=12$ does not hide another solution of the coefficient equation. The [Routh-Hurwitz stability criterion](../../../../../../routh-hurwitz-stability-criterion.md) shows that both [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are stable for $0<d<1$, $c_H^*(d)<c<d$, and unstable for $c<c_H^*(d)$. For $d\ge1$, $3c/d-d-2<1-d\le0$, so no nonzero [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) is stable.

Their [Hopf bifurcations](../../../../../../hopf-bifurcation.md) are supercritical. Here is a coefficient check that includes the effect of the quadratic term around $x_*$. Let $B_2(u,v)=2x_*u_xv_x$, $C_2(u,v,w)=2u_xv_xw_x$ and normalize $q_x=1$ as before. The inverse-linearization term has $(L^{-1}B(q,\bar q))_x=3/x_*$. Also

$$
G_2={2i\omega-d/2\over-3\omega^2(\tau+2i\omega)},\qquad
((2i\omega I-L)^{-1}B(q,q))_x=2x_*G_2.
$$

The resonant cubic Hopf coefficient is

$$
l_1={1\over2\omega}\operatorname{Re}\{G[-10+4x_*^2G_2]\}
=-{8[d(4-d)^2+(28d+48)\omega^2]\over d\omega[(4-d)^2+4\omega^2][(4-d)^2+16\omega^2]}<0.
$$

In this simplification $x_*^2/\omega^2=3\tau/d$. Thus stable small [periodic orbits](../../../../../../periodic-orbit.md) appear around each nonzero [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) on the $c<c_H^*(d)$ side. This classifies the local branches; the sketch does not infer uncomputed distant global bifurcations.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
