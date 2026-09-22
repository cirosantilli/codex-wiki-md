<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Set $\xi=x/t^\beta$ and $u=t^\alpha F(\xi)$. Balancing $u_t$, [diffusion](../../../../diffusion.md) and the cubic gives $\alpha-1=\alpha-2\beta=3\alpha$, hence $\boxed{\alpha=-1/2,\quad\beta=1/2}$. The drift term cancels the $-\beta\xi F'$ contribution in $u_t$, leaving

$$
F''+\tfrac12F-\tfrac12F^3=0,\qquad F(0)=0,\quad F(+\infty)=1.
$$

Multiply by $F'$ and integrate. The limiting [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) has $F'=0$, fixing the constant and giving $(F')^2=(1-F^2)^2/4$. The increasing branch from zero to one obeys $F'=(1-F^2)/2$. Therefore

$$
\boxed{F(\xi)=\tanh(\xi/2),\qquad
u(x,t)=t^{-1/2}\tanh\!\left(\frac{x}{2\sqrt t}\right).}
$$

The [first integral](../../../../first-integral.md) also shows why another turning branch cannot reach the required limit from zero.

At a space-time interior maximum, $u_t=u_x=0$ and $u_{xx}\leq0$. The equation would then give $0=u_{xx}-u^3/2$, so $u\leq0$. Hence **a positive interior maximum is impossible**. In particular, a [global maximum](../../../../global-maximum.md) cannot be attained at an interior point, since the far-field boundary has positive values. If “maximum” instead means every [local maximum](../../../../local-maximum.md) of an arbitrary signed solution, the calculation only excludes positive local maxima; nonnegativity must be added for the broader usual interpretation. Positive boundary values alone do not impose nonnegativity on arbitrary [initial data](../../../../initial-data-in-general-relativity.md).

For uniqueness in the standard bounded [classical solution](../../../../classical-solution.md) class on finite time strips, set $\tau=\log t$, $\xi=x/\sqrt t$, and $v(\xi,\tau)=\sqrt t\,u(x,t)$. The equation becomes

$$
v_\tau=v_{\xi\xi}+\tfrac12v-\tfrac12v^3,
$$

with $v(0,\tau)=0$, $v(\infty,\tau)=1$ and prescribed $v(\xi,0)=f(\xi)$. For two solutions let $w=v_1-v_2$. Then

$$
w_\tau=w_{\xi\xi}+\left[\tfrac12-\tfrac12(v_1^2+v_1v_2+v_2^2)\right]w.
$$

The bracket is at most $1/2$ since $a^2+ab+b^2\geq0$. Thus $z=e^{-\tau/2}w$ solves $z_\tau=z_{\xi\xi}-Qz$ with $Q=(v_1^2+v_1v_2+v_2^2)/2\geq0$, zero [initial data](../../../../initial-data-in-general-relativity.md) and zero boundary difference.

For completeness on the unbounded interval, compare $\pm z$ with $\eta e^{3\tau}(1+\xi^2)$ on a large rectangle. This is a strict positive [supersolution](../../../../supersolution.md) because

$$
(\partial_\tau-\partial_{\xi\xi}+Q)e^{3\tau}(1+\xi^2)
=e^{3\tau}[3(1+\xi^2)-2+Q(1+\xi^2)]>0.
$$

Finite-strip boundedness lets its right boundary dominate $z$ when the rectangle is sufficiently wide. The [weak parabolic maximum principle](../../../../weak-parabolic-maximum-principle.md) then bounds $|z|$ by this barrier. Send the width to infinity and then $\eta$ to zero. Hence $z=w=0$, giving $\boxed{\text{at most one bounded classical solution for }t>1}$. The boundedness or a suitable uniform far-field/growth condition is the usual hypothesis that makes this unbounded-domain argument valid; pointwise limits at [spatial infinity](../../../../spatial-infinity.md) should not silently replace it. This is [similarity reduction for a cubic absorption equation with dilating drift](../../../../similarity-reduction-for-a-cubic-absorption-equation-with-dilating-drift.md).

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the differential equations and applications course of the University of Oxford](../../../split.md)
5. [Differential equations and applications course of the University of Oxford](../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
