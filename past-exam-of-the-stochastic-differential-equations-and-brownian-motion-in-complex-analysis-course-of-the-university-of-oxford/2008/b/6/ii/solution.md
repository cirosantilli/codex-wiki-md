<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[planar Brownian motion](../../../../../planar-brownian-motion.md) is [recurrence of planar Brownian motion](../../../../../recurrence-of-planar-brownian-motion.md) when, almost surely, it returns to every nonempty open neighborhood infinitely often, at arbitrarily large times. This does not mean that it hits each specified point; a prescribed point is polar for [planar Brownian motion](../../../../../planar-brownian-motion.md).

[recurrence of planar Brownian motion](../../../../../recurrence-of-planar-brownian-motion.md) and [continuity](../../../../../continuous-function.md) imply that all the circle-hitting times $S_k,T_k$ in the question are finite. Starting on radius $\epsilon$, it eventually visits the exterior of radius $2\epsilon$ and must cross that circle; it later visits the interior of radius $\epsilon$ and must cross back. Each duration $\Delta_k=T_k-S_k$ is strictly positive by path [continuity](../../../../../continuous-function.md), because the two radii are separated.

At $S_k$, the [Strong Markov property](../../../../../strong-markov-property.md) restarts [Brownian motion](../../../../../brownian-motion-split.md) at its current point on the inner circle. [rotational invariance of Brownian motion](../../../../../rotational-invariance-of-brownian-motion.md) makes the law of the subsequent first exit time from the radius-$2\epsilon$ disk independent of that starting angle. Its conditional distribution given the past is therefore the same fixed law at every cycle, proving that the $\Delta_k$ are independent and identically distributed.

To prove divergence of the conformal clock for any nonconstant entire $f$, choose a point $z_0$ with $f'(z_0)\neq0$. By [continuity](../../../../../continuous-function.md), there exist $\rho,c>0$ such that $|f'(z)|^2\geq c$ throughout the closed disk $|z-z_0|\leq2\rho$. Use the same [recurrence of planar Brownian motion](../../../../../recurrence-of-planar-brownian-motion.md) circle cycles centered at $z_0$, with radii $\rho,2\rho$. On each segment from the inner circle to the outer circle, the path remains in that disk, giving

$$
\int_0^\infty|f'(Z_s)|^2ds
\geq c\sum_{k\geq0}(T_k-S_k).
$$

The durations are positive iid variables. If their mean has not been computed, apply the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) to the bounded iid variables $\min(\Delta_k,1)$: their mean is strictly positive, so their sum, and hence $\sum\Delta_k$, diverges almost surely. Therefore

$$
\boxed{\int_0^\infty|f'(Z_s)|^2ds=\infty\quad\text{almost surely}.}
$$

Centering the disks at a noncritical point avoids an unjustified positive lower bound on $|f'|$ around the original origin.

Write $f=u+iv$. Harmonicity and [Itô's formula](../../../../../ito-s-lemma.md) make $u(Z_t),v(Z_t)$ continuous [local martingales](../../../../../local-martingale.md). The [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) give equal brackets $\int_0^t|f'(Z_s)|^2ds$ and zero mutual bracket. Consequently [Lévy's characterization of Brownian motion](../../../../../levy-characterization-of-brownian-motion.md) after [time change of a continuous process](../../../../../time-change-of-a-continuous-process.md) makes $W$ a [planar Brownian motion](../../../../../planar-brownian-motion.md) started at $f(Z_0)$, with no finite clock lifetime because the clock just proved is unbounded. The clock is strictly increasing: otherwise $f'$ would vanish along a nonconstant path interval, contradicting its isolated zeros.

For the notation in the source, $|\nabla f|^2$ is interpreted as the conformal scale $|f'|^2=|\nabla u|^2=|\nabla v|^2$. If it instead means the sum of the squared magnitudes of both complex coordinate derivatives, it is $2|f'|^2$, and the resulting $W$ runs at half the usual Brownian speed. This convention does not change divergence of the integral. The mechanism is [recurrent disk occupation makes an entire conformal clock infinite](../../../../../recurrent-disk-occupation-makes-an-entire-conformal-clock-infinite.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
