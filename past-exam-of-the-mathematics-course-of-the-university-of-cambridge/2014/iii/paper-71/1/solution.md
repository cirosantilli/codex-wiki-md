<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The dimensional [linear friction coefficient](../../../../../linear-friction-coefficient.md) is $\zeta$. Put $y=x-v_Tt$ and $u(y)=F(y)/\zeta$. In [overdamped particle dynamics](../../../../../overdamped-particle-dynamics.md) the laboratory [velocity](../../../../../velocity.md) is $\dot x=u(y)$, whereas the trap-frame [velocity](../../../../../velocity.md) is $\dot y=u(y)-v_T$. The particle enters the [optical tweezers](../../../../../optical-tweezers.md) at $y=X_R$ and leaves at $y=-X_L$ when the trap overtakes it. Write $w=X_R+X_L$ for this support width. **The printed subtraction in the later definition of the width is a sign error:** the distance between these endpoints is their sum. We use $w=2X_0$ in the circular calculation.

For a bounded continuous [force](../../../../../force.md), the strict condition

$$
\boxed{v_T>\max_y u(y)=\max_y F(y)/\zeta}
$$

ensures finite [passage through a translating optical trap](../../../../../passage-through-a-translating-optical-trap.md): the trap-frame coordinate decreases throughout the interaction. If $u(y)=v_T$ is encountered from the right, the deterministic trajectory cannot pass this stationary trap-frame point for a locally Lipschitz [force](../../../../../force.md); it approaches or stays at a locked state. At a smooth maximum the critical passage time diverges. More generally the passage criterion is $v_T-u>0$ on the traversed interval together with a finite integral below. Separating the trap-frame equation gives

$$
\boxed{\Delta t=\int_{-X_L}^{X_R}\frac{dy}{v_T-u(y)},\qquad
\Delta x=\int_{-X_L}^{X_R}\frac{u(y)}{v_T-u(y)}\,dy
=v_T\Delta t-w.}
$$

These formulas account for both portions of the [optical tweezers](../../../../../optical-tweezers.md), including motion against the trap direction.

The forward-displacement result uses the ordinary localized [potential energy](../../../../../potential-energy.md) interpretation of an [optical trap](../../../../../optical-tweezers.md): $F=-U'$ and $U$ has the same value outside both ends, hence $\int F\,dy=0$. [Compact support](../../../../../compact-support.md) of the [force](../../../../../force.md) alone does not ensure that condition. Under the equal-endpoint condition,

$$
\frac{u}{v_T-u}=\frac{u}{v_T}+\frac{u^2}{v_T(v_T-u)},\qquad
\boxed{\Delta x=\frac1{v_T}\int_{-X_L}^{X_R}\frac{u(y)^2}{v_T-u(y)}\,dy>0}
$$

for a nonzero [force](../../../../../force.md) and a passing trajectory. This is [forward displacement from a translating localized potential](../../../../../forward-displacement-from-a-translating-localized-potential.md). A zero [force](../../../../../force.md) gives zero displacement. If the [force](../../../../../force.md) is negative everywhere on its support, it instead gives $\Delta x<0$; thus an arbitrary compactly supported [force](../../../../../force.md) does not satisfy the printed assertion.

There are two complementary explanations of the [forward displacement from a translating localized potential](../../../../../forward-displacement-from-a-translating-localized-potential.md). The forward push slows the relative passage and therefore acts longer, while the backward pull speeds up the relative passage and therefore acts for less time. An exact [potential energy](../../../../../potential-energy.md) balance makes the same point: along the trajectory

$$
\frac{dU(y)}{dt}=-\zeta\dot x^2+\zeta v_T\dot x,
\qquad
\boxed{\zeta v_T\Delta x=\zeta\int_{\mathrm{interaction}}\dot x^2\,dt.}
$$

The moving [optical trap](../../../../../optical-tweezers.md) supplies the positive work lost to [linear drag](../../../../../linear-drag.md), although the initial and final [potential energy](../../../../../potential-energy.md) are equal.

For $v_T\gg\|u\|_\infty$, a uniformly convergent expansion of the passage integrals gives

$$
\Delta x=\frac1{v_T}\int u\,dy+\frac1{v_T^2}\int u^2\,dy+O(v_T^{-3}).
$$

For a localized [potential energy](../../../../../potential-energy.md) well the first integral vanishes, so

$$
\boxed{\Delta x\sim\frac1{\zeta^2v_T^2}\int_{-X_L}^{X_R}F(y)^2\,dy,\qquad
\Delta t=\frac w{v_T}+\frac1{\zeta^2v_T^3}\int F(y)^2\,dy+O(v_T^{-4}).}
$$

The displacement decreases quadratically with the trap speed, rather than linearly. Without the equal-endpoint assumption the general expansion above remains valid.

For [repeated kicks from a circular optical trap](../../../../../repeated-kicks-from-a-circular-optical-trap.md), let $L=2\pi R$ and interpret the [force](../../../../../force.md) profile locally along the arc. This description requires a tangential constraint, a nonoverlapping [force](../../../../../force.md) support $w<L$, and, if the straight profile is used geometrically, a small support compared with $R$. The condition $R\gg a$ alone does not specify that latter width hierarchy. During an encounter the particle advances by $\Delta x$ and the trap advances by $v_T\Delta t=w+\Delta x$. Between encounters the deterministic particle is stationary and the trap travels the remaining relative distance $L-w$. Thus the time between corresponding points of successive encounters is

$$
T_{\mathrm{kick}}=\Delta t+\frac{L-w}{v_T},\qquad
\boxed{f_p=\frac{\Delta x/L}{\Delta t+(L-w)/v_T}
=\frac{(\Delta x/L)f_T}{1+f_T\Delta t-w/L}
=\frac{\Delta x}{L+\Delta x}f_T.}
$$

Here $f_T$ and $f_p$ are revolution [frequencies](../../../../../frequency.md), not angular velocities; the printed relation $f_T=v_T/(2\pi R)$ fixes this convention. The encounter [frequency](../../../../../frequency.md) is $f_T-f_p$, so the same result follows from $Lf_p=\Delta x(f_T-f_p)$.

The precise condition for the stated approximation is $|\Delta x|/L\ll1$, in addition to finite passage and separated encounters. A sufficient high-speed regime is $v_T\gg\|F\|_\infty/\zeta$ with fixed $w<L$, for which the asymptotic displacement divided by $L$ tends to zero. Then

$$
\boxed{f_p\simeq\frac{\Delta x}{2\pi R}f_T.}
$$

This condition controls the encounter [frequency](../../../../../frequency.md) correction; there is no need to discard the finite interaction time without accounting for the support width.

For the [triangular optical-trap response](../../../../../triangular-optical-trap-response.md), set $v_c=F/\zeta=Lf_c$. In the passing regime $v_T>v_c$, the approach side has [velocity](../../../../../velocity.md) $-v_c$ and the trailing side has [velocity](../../../../../velocity.md) $+v_c$. Consequently

$$
\Delta t=\frac{X_0}{v_T+v_c}+\frac{X_0}{v_T-v_c}
=\frac{2X_0v_T}{v_T^2-v_c^2},\qquad
\Delta x=\frac{2X_0v_c^2}{v_T^2-v_c^2}.
$$

With $\alpha=2X_0/L=X_0/(\pi R)$ and $\beta=v_T/v_c=f_T/f_c$, the [repeated kicks from a circular optical trap](../../../../../repeated-kicks-from-a-circular-optical-trap.md) formula becomes

$$
\boxed{\frac{f_p}{f_c}=\frac{\alpha\beta}{\beta^2-1+\alpha}\quad(\beta>1).}
$$

For $0<\beta<1$ the usual ideal triangular-well dynamics locks at the cusp: the forces on its two sides direct the trap-frame particle towards the cusp. This is understood as the sticking limit of a rounded potential or of the overdamped differential inclusion at its discontinuous [force](../../../../../force.md). The particle follows the trap, giving $f_p/f_c=\beta$. At $\beta=1$ it can remain at a fixed point of the trailing segment and also has $f_p/f_c=1$. Thus the physical [triangular optical-trap response](../../../../../triangular-optical-trap-response.md) is continuous at threshold, even though the isolated passing-kick displacement diverges there. For $\beta\gg1$,

$$
\boxed{f_p/f_c\sim\alpha/\beta,}
$$

and the more general kick approximation requires $\alpha/(\beta^2-1)\ll1$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
