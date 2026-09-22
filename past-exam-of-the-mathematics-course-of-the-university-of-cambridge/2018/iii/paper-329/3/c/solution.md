<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the horizontal film, part (a) gives the [lubrication theory](../../../../../../lubrication-theory.md) equation

$$
h_t=K(h^3h_x)_x,\qquad K=\frac{\rho g}{3\mu}.
$$

The length scale is fixed at $L$, so balancing $h/t$ against $Kh^4/L^2$ gives $h\sim(L^2/(Kt))^{1/3}$. The [draining viscous film on a finite horizontal plate](../../../../../../draining-viscous-film-on-a-finite-horizontal-plate.md) therefore has the long-time [similarity solution](../../../../../../similarity-solution.md)

$$
\boxed{h(x,t)=\left(\frac{L^2}{Kt}\right)^{1/3}H(\eta),\qquad
\eta=\frac xL,\qquad h\propto t^{-1/3}.}
$$

An additive shift of the time origin can represent the initial transient without changing the long-time law. The positive profile is even, with $H'(0)=0$ and $H(\pm1)=0$. Substitution yields

$$
(H^3H')'=-\frac H3.
$$

To integrate, put $q=H^3H'$ and use $q'=q\,dq/dH\,/H^3$. Then

$$
q\frac{dq}{dH}=-\frac{H^4}{3},\qquad
q^2=\frac2{15}(H_0^5-H^5),\qquad H_0=H(0).
$$

For $0<\eta<1$ the decreasing branch has $q<0$, so inversion gives

$$
\boxed{\eta(H)=\int_H^{H_0}F(s)\,ds,\qquad
F(s)=\sqrt{\frac{15}{2}}\frac{s^3}{\sqrt{H_0^5-s^5}}.}
$$

The negative half of the profile follows by symmetry.

At the edge, $\eta(0)=1$. Set $u=(s/H_0)^5$ in the integral to obtain

$$
1=\frac15\sqrt{\frac{15}{2}}H_0^{3/2}
\int_0^1u^{-1/5}(1-u)^{-1/2}\,du
=\frac15\sqrt{\frac{15}{2}}H_0^{3/2}C,
\qquad C=B(4/5,1/2).
$$

Here $B$ is the [beta function](../../../../../../beta-function.md). Thus $H_0^3=10/(3C^2)$, and the centre thickness is

$$
\boxed{h_0(t)=h(0,t)=\left(\frac{10\mu L^2}{\rho gC^2t}\right)^{1/3}.}
$$

For $H\ll H_0$, the implicit integral remaining between $0$ and $H$ gives

$$
1-\eta\sim\sqrt{\frac{15}{2}}\frac{H^4}{4H_0^{5/2}},\qquad
\left(\frac H{H_0}\right)^4\sim\frac{4C}{5}(1-\eta).
$$

Consequently the [edge region of a draining viscous film](../../../../../../edge-region-of-a-draining-viscous-film.md) has

$$
\boxed{k=\frac14,\qquad
h\sim h_0\left[\frac{4C}{5}\frac{L-x}{L}\right]^{1/4}.}
$$

Its slope satisfies $|h_x|\sim(h_0/L)(1-x/L)^{-3/4}$ up to a constant factor, so it becomes order one at

$$
\boxed{\ell=L-x\sim L\left(\frac{h_0}{L}\right)^{4/3}.}
$$

The local height is then also $O(\ell)$, violating the shallow geometry required by [lubrication theory](../../../../../../lubrication-theory.md). A full local flow is needed to turn the fluid over the edge.

The imposed zero thickness is nevertheless a consistent leading outer boundary condition: $\ell/h_0\sim(h_0/L)^{1/3}\ll1$, so the unresolved edge height is small compared with the film's bulk height. It should not be interpreted as an exact pointwise prediction inside the edge region. Moreover, $H^3H'\to-\sqrt{2/15}\,H_0^{5/2}$ at the right edge, so the outward [volume flux](../../../../../../volumetric-flow-rate.md) remains finite even as the outer thickness tends to zero. The singular slope is what allows this outer solution to describe drainage.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
