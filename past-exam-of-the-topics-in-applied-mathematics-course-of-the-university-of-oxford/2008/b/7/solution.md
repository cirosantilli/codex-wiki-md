<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For $r>0$, differentiate $r^2=x^2+y^2$ and use the two differential equations:

$$
\dot r=\frac{x\dot x+y\dot y}{r}=r(a-f(x,y)),\qquad
\dot\theta=\frac{x\dot y-y\dot x}{r^2}=1.
$$

Substituting $x=r\cos\theta$, $y=r\sin\theta$ gives the required equations in [polar coordinates](../../../../polar-coordinates.md). The origin is handled in [Cartesian coordinates](../../../../cartesian-coordinate-system.md), where it is an [equilibrium point](../../../../equilibrium-point-of-a-dynamical-system.md); an angular coordinate is not defined there.

A [Lyapunov function](../../../../lyapunov-function.md) near an [equilibrium point](../../../../equilibrium-point-of-a-dynamical-system.md) is a continuously differentiable [positive-definite scalar function](../../../../positive-definite-scalar-function.md) $V$ whose [derivative](../../../../derivative.md) along solutions is nonpositive. This implies local [Lyapunov stability](../../../../lyapunov-stability.md) under the usual comparison bounds; if its [derivative](../../../../derivative.md) is negative definite, the [Second Lyapunov theorem](../../../../second-lyapunov-theorem.md) gives local [asymptotic stability](../../../../asymptotic-stability.md). Here take

$$
V(x,y)=\frac12(x^2+y^2),\qquad \dot V=r^2(a-f(x,y)).
$$

If $a<f(0,0)$, continuity gives a small ball and $\delta>0$ such that $f(x,y)-a\ge\delta$ inside it. Consequently $\dot V\le-2\delta V$. A sufficiently small initial sublevel set stays inside the ball, and $V(t)\le V(0)e^{-2\delta t}$. **The origin is [asymptotically stable](../../../../asymptotic-stability.md)**, in fact locally [exponentially stable](../../../../exponential-stability.md). If $a>f(0,0)$, continuity instead gives $\dot V\ge2\delta V$ in a small ball. Every nonzero initial point there exits that ball in forward time, proving **[instability](../../../../instability.md) of the origin**. These inequalities hold along all local solutions; continuity of $f$ alone need not supply uniqueness for a general [vector field](../../../../vector-field.md).

If $f=g(r)$, a nonzero constant radius $r_0$ satisfying $a=g(r_0)$ gives a [periodic orbit](../../../../periodic-orbit.md) of period $2\pi$, since $\dot\theta=1$. Linearizing the scalar radial equation there gives

$$
\dot\rho=-r_0g'(r_0)\rho+O(\rho^2).
$$

Thus the [periodic orbit](../../../../periodic-orbit.md) is [orbitally asymptotically stable](../../../../orbital-asymptotic-stability.md) for $g'(r_0)>0$ and [unstable](../../../../instability.md) for $g'(r_0)<0$. The direction along the [periodic orbit](../../../../periodic-orbit.md) is neutral, as expected for an autonomous [periodic orbit](../../../../periodic-orbit.md); [orbital asymptotic stability](../../../../orbital-asymptotic-stability.md) means [attraction in a dynamical system](../../../../attraction-in-a-dynamical-system.md) to the orbit with a possible phase shift.

For the specified radial response,

$$
g(0)=\frac32,\qquad g'(r)=\frac{-2(r-1)}{[1+(r-1)^2]^2}.
$$

The origin is therefore [stable](../../../../lyapunov-stability.md) for $0<a<3/2$ and [unstable](../../../../instability.md) for $a>3/2$. The nonzero-radius equation has [roots of an equation](../../../../root-of-an-equation.md)

$$
\boxed{r_\pm=1\pm\sqrt{\frac{2-a}{a-1}},\qquad1<a\le2,}
$$

retaining only positive radii. For $1<a<3/2$, the [square root](../../../../square-root.md) exceeds one, so only $r_+>1$ exists and $g'(r_+)<0$: the [periodic orbit](../../../../periodic-orbit.md) is [unstable](../../../../instability.md). For $3/2<a<2$, both radii are positive; $0<r_-<1$ gives $g'(r_-)>0$ and a [stable](../../../../lyapunov-stability.md) [periodic orbit](../../../../periodic-orbit.md), while $r_+>1$ remains [unstable](../../../../instability.md).

As $a$ increases through $3/2$, the [stable](../../../../lyapunov-stability.md) small-radius [periodic orbit](../../../../periodic-orbit.md) emerges from the origin while the origin loses [Lyapunov stability](../../../../lyapunov-stability.md). This is the supercritical [Hopf-type transition with a nonsmooth radial response](../../../../hopf-type-transition-with-a-nonsmooth-radial-response.md) requested. It follows directly from the explicit radial dynamics. There is a regularity qualification: $g(r)=3/2+r/2+O(r^2)$ near zero, so the [vector field](../../../../vector-field.md) in [Cartesian coordinates](../../../../cartesian-coordinate-system.md) contains $x\sqrt{x^2+y^2}$ and $y\sqrt{x^2+y^2}$ terms. It is continuously differentiable but not generally twice differentiable at the origin, and the [periodic orbit](../../../../periodic-orbit.md) radius grows as $r_-\sim2(a-3/2)$ rather than the square-root law of a generic smooth [Hopf normal form](../../../../hopf-normal-form.md). One should therefore use the explicit computation here rather than invoke a smooth [Hopf bifurcation](../../../../hopf-bifurcation.md) theorem with unmet hypotheses. At $a=3/2$ itself the origin is still weakly [attracting](../../../../attraction-in-a-dynamical-system.md), because $a-g(r)<0$ for small positive $r$.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../split.md)
5. [Topics in applied mathematics course of the University of Oxford](../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
