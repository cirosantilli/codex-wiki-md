<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [first-order phase transition](../../../../../../first-order-phase-transition.md) has a discontinuity in a first derivative of the equilibrium [free energy](../../../../../../thermodynamic-free-energy.md), such as the [entropy](../../../../../../entropy.md) or [order parameter](../../../../../../order-parameter.md). It can have latent heat when the [entropy](../../../../../../entropy.md) jumps. A [continuous phase transition](../../../../../../continuous-phase-transition.md) has a continuously vanishing [order parameter](../../../../../../order-parameter.md) and no latent heat, with singular higher derivatives and a diverging [correlation length](../../../../../../correlation-length.md). The [LG theory](../../../../../../landau-ginzburg-theory.md) compares [global minima](../../../../../../global-minimum.md), not merely the points where a local minimum loses stability.

For the uniform quartic [Landau free energy](../../../../../../landau-free-energy.md)

$$
V(m)=\tfrac12rm^2+\tfrac14um^4-hm,\qquad u>0,
$$

the [equation of state](../../../../../../equation-of-state.md) is $rm+um^3=h$. At zero field the stable minimum is $m=0$ for $r>0$, and $m=\pm\sqrt{-r/u}$ for $r<0$. Thus tuning $r$ through zero gives a **continuous transition**. For a fixed $r<0$, varying $h$ through zero instead switches between the two ordered minima and makes $m$ jump, giving a [first-order phase transition](../../../../../../first-order-phase-transition.md) in the [conjugate field](../../../../../../field-conjugate-to-an-order-parameter.md).

A temperature-like first-order transition can occur at zero field when $u<0$ and a positive sextic term $vm^6/6$ stabilizes the potential. Write $q=m^2$. Stationarity of a nonzero phase gives $r+uq+vq^2=0$, while equality with $V(0)=0$ gives $rq/2+uq^2/4+vq^3/6=0$. Solving these two conditions yields

$$
\boxed{q_{\rm coex}=-\frac{3u}{4v},\qquad r_{\rm coex}=\frac{3u^2}{16v}\quad(u<0).}
$$

The [order parameter](../../../../../../order-parameter.md) jumps from zero to $\pm\sqrt{q_{\rm coex}}$. At this point

$$
V(m)=\frac v6m^2\left(m^2+\frac{3u}{4v}\right)^2\geq0,
$$

so the competing stationary points are genuinely [global minima](../../../../../../global-minimum.md). This [phase coexistence](../../../../../../phase-coexistence.md) condition differs from the [spinodal points](../../../../../../spinodal-point.md) $r=0$ and $r=u^2/(4v)$, which mark loss or creation of local stability, not equilibrium coexistence.

If the symmetry permits a cubic term $wm^3/3$, a positive quartic coefficient does not preclude a first-order transition. For $V=rm^2/2+wm^3/3+um^4/4$ with $w\ne0,u>0$, stationarity and coexistence give $m=-2w/(3u)$ and $r=2w^2/(9u)$. This is the [first-order transition in a cubic-quartic Landau potential](../../../../../../first-order-transition-in-a-cubic-quartic-landau-potential.md); the symmetry restriction on the expansion is therefore part of the prediction.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
