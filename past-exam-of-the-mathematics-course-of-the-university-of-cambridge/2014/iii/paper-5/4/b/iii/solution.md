<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix $u_l>u_r$ and the [Rankine-Hugoniot condition](../../../../../../../rankine-hugoniot-conditions.md) speed from the preceding part. The new hypothesis is a [uniformly convex scalar flux](../../../../../../../uniformly-convex-scalar-flux.md), $F''\geq\kappa>0$; it replaces the globally bounded-$F'$ hypothesis of part (a). Choose $b=\sigma u_r-F(u_r)$. Then

$$
Q(z)=F(z)-\bigl(F(u_r)+\sigma(z-u_r)\bigr)<0\quad(u_r<z<u_l),
$$

since a strictly [convex function](../../../../../../../convex-function.md) lies below the chord between its two endpoint values. Also $Q(u_l)=Q(u_r)=0$ and

$$
F'(u_r)<\sigma<F'(u_l).
$$

The zeros at the endpoints are simple, so the separated integral diverges logarithmically there. Thus the [travelling wave](../../../../../../../travelling-wave.md) is a decreasing connection defined for all $s$, unique up to translation.

To specify a limit, fix a number $c\in(u_r,u_l)$ independently of $\varepsilon$ and normalize $v_\varepsilon(0)=c$. If $V'=Q(V)$ and $V(0)=c$, uniqueness gives $v_\varepsilon(s)=V(s/\varepsilon)$. Consequently

$$
\boxed{u_\varepsilon(t,x)\longrightarrow
\begin{cases}u_l,&x<\sigma t,\\u_r,&x>\sigma t.\end{cases}}
$$

At $x=\sigma t$ the normalized profile equals $c$ for every $\varepsilon$. This single-line value is immaterial to the [weak solution](../../../../../../../weak-solution.md). Convergence holds pointwise off the line and in $L^1_{\mathrm{loc}}$ by bounded convergence; it cannot be uniform across a nonzero jump. The transition has thickness of order $\varepsilon$.

This is the [vanishing viscosity approximation](../../../../../../../vanishing-viscosity-approximation.md) to a compressive [entropy shock](../../../../../../../entropy-shock.md). The [Rankine-Hugoniot condition](../../../../../../../rankine-hugoniot-conditions.md) makes the step a [weak solution](../../../../../../../weak-solution.md) of the inviscid [scalar conservation law](../../../../../../../scalar-conservation-law.md), while $F'(u_r)<\sigma<F'(u_l)$ means [characteristic curves](../../../../../../../characteristic-curve.md) enter the shock from both sides. For every [smooth](../../../../../../../smooth-function.md) [convex function](../../../../../../../convex-function.md) $\eta$ used as an entropy, with [entropy flux for a scalar conservation law](../../../../../../../entropy-flux-for-a-scalar-conservation-law.md) $q'=\eta'F'$, the viscous equation gives

$$
\partial_t\eta(u)+\partial_xq(u)
=\varepsilon\partial_{xx}\eta(u)-\varepsilon\eta''(u)u_x^2
\leq\varepsilon\partial_{xx}\eta(u).
$$

Against compactly supported tests the right side tends to zero, since $u_\varepsilon$ stays in $[u_r,u_l]$. Passing to the $L^1_{\mathrm{loc}}$ limit yields the entropy inequality, explaining the direction selected by positive viscosity.

**A translation must be fixed to obtain this particular limit.** An $\varepsilon$-dependent translate $V((s-a_\varepsilon)/\varepsilon)$ can converge to a shock at a different location, to a constant if its center escapes, or fail to converge if the centers oscillate. Thus existence of profiles alone does not specify a single vanishing-viscosity limit without a phase normalization.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
