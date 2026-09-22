<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a starting price above the trigger, maximizing $V_L(S)$ amounts to maximizing $g(L)=(X-L)L^{-\beta_-}$ on $0<L<X$. Its derivative is

$$
g'(L)=L^{-\beta_--1}\bigl[(\beta_--1)L-\beta_-X\bigr].
$$

Because $\beta_-<0$, this is positive below $\beta_-X/(\beta_--1)$ and negative above it. Both endpoint limits of $g$ are zero. Thus the unique maximizing trigger is

$$
\boxed{S^*=\frac{\beta_-}{\beta_--1}X,\qquad 0<S^*<X.}
$$

Equivalently [smooth fit](../../../../../../smooth-pasting.md) requires $\beta_-(X-S^*)/S^*=-1$, matching the derivative of $X-S$ below the boundary. The optimized [perpetual put option](../../../../../../perpetual-put-option.md) value is $X-S$ for $S\le S^*$ and $(X-S^*)(S/S^*)^{\beta_-}$ above it.

We can verify optimality among all stopping rules, not only constant triggers. The continuation branch is convex, with value and slope matching $X-S$ at $S^*$, so it dominates $X-S$ above the boundary; it is also positive, and hence dominates $(X-S)^+$ everywhere. Its discounted generator vanishes in continuation. In the exercise region, the generator of $X-S$ is $\delta S-rX$. The root equation gives

$$
\delta S^*/X=r+\tfrac12\sigma^2\beta_-<r,
$$

so for $\delta\ge0$ this generator is nonpositive throughout $S\le S^*$. [Smooth fit](../../../../../../smooth-pasting.md) eliminates a local-time contribution at the boundary. [Itô formula](../../../../../../ito-s-lemma.md) and localization therefore make $e^{-rt}V(S_t)$ a nonnegative [supermartingale](../../../../../../supermartingale.md), providing an upper bound for every discounted exercise payoff. The threshold strategy attains that bound by the [martingale](../../../../../../martingale-split.md) calculation in part (a). This proves the boundary is globally optimal.

The positive-interest assumption is substantive. If $r=0$ and $\delta\ge0$, the [stock](../../../../../../stock.md) tends to zero almost surely, so the [supremum](../../../../../../supremum.md) of perpetual put payoffs has value $X$, approached by triggers $L\downarrow0$. No positive finite trigger attains that [supremum](../../../../../../supremum.md) for positive spot. The displayed finite-boundary formula belongs to the $r>0$ case. If $r<0$ and $\delta\ge0$, the [stock](../../../../../../stock.md) still tends to zero, while the [discount factor](../../../../../../discount-factor.md) grows without bound. Even exercise at deterministic times tending to infinity makes the expected discounted put payoff unbounded, so there is no finite perpetual price in that extension.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
