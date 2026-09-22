<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

Take $0\le\gamma\le1$ for the [coefficient of restitution](../../../../../coefficient-of-restitution.md). [Conservation of energy](../../../../../conservation-of-energy.md) in the initial vacuum fall gives

$$
\boxed{u_0=\sqrt{2gh_0}.}
$$

The fixed plate has zero velocity, so the restitution rule makes the first upward rebound speed $u_1=\gamma u_0$. The ratio of rebound to impact [kinetic energy](../../../../../kinetic-energy.md) is $\gamma^2$; hence

$$
\boxed{u_1=\gamma\sqrt{2gh_0},\qquad\text{fraction dissipated}=1-\gamma^2.}
$$

Gravity preserves the speed magnitude between departure from and return to the same plate height. Therefore the upward speed after the $n$th bounce is $\gamma^n u_0$. The [geometric bounce sequence](../../../../../geometric-bounce-sequence.md) has

$$
\boxed{h_n=\gamma^{2n}h_0,\qquad T_n=\frac{2\gamma^n u_0}{g}=2\gamma^n\sqrt{\frac{2h_0}{g}}\quad(n\ge1).}
$$

The total travelled distance for $\gamma<1$ is the first fall plus ascent and descent for every rebound. Summing the [geometric series](../../../../../geometric-series.md) gives

$$
\boxed{D=h_0+2\sum_{n=1}^{\infty}h_0\gamma^{2n}
=h_0\frac{1+\gamma^2}{1-\gamma^2}.}
$$

The idealized infinitely many impacts accumulate in finite time, after which the limiting state is rest on the plate; $\gamma=0$ gives rest at the first impact.

For the atmospheric fall, use upward signed velocity $u$ and height $z$. [Newtonian mechanics](../../../../../newtonian-mechanics.md) with [quadratic drag](../../../../../quadratic-drag.md) gives

$$
m\dot u=-mg-\alpha|u|u,\qquad u(0)=0,\qquad z(0)=h_0.
$$

Before impact $u\le0$, so $\dot u=-g+(\alpha/m)u^2$. Set $v=-u\ge0$, $v_T=\sqrt{mg/\alpha}$, and $\beta=\sqrt{\alpha g/m}=g/v_T$. Separation gives $\operatorname{artanh}(v/v_T)=\beta t$, establishing the [descent from rest under quadratic drag](../../../../../descent-from-rest-under-quadratic-drag.md):

$$
\boxed{u(t)=-\sqrt{\frac{mg}{\alpha}}\tanh\!\left(\sqrt{\frac{\alpha g}{m}}\,t\right),\qquad
z(t)=h_0-\frac m\alpha\log\cosh(\beta t).}
$$

The speed approaches the [terminal velocity](../../../../../terminal-velocity.md) $v_T$, although the formula is used only until the first impact. This occurs when $\cosh(\beta t_{{\rm hit}})=e^{\alpha h_0/m}$. In particular, the atmospheric impact speed is $v_T\sqrt{1-e^{-2\alpha h_0/m}}$, and both speed and height formulas recover the vacuum fall as $\alpha\to0$.

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
