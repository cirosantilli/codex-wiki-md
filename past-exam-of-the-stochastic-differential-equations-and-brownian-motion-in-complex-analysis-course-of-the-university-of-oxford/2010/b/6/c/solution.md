<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The second coordinate $\zeta^2$ is one-dimensional [Brownian motion](../../../../../brownian-motion-split.md), whose zero set is unbounded almost surely by recurrence. The clock $\tau$ and its inverse are continuous, increasing, and unbounded, so the unwrapped angle $\Theta_t=\zeta^2_{\tau(t)}$ has zeros at arbitrarily large original times.

To ensure the times are [stopping times](../../../../../stopping-time.md) for the original Brownian filtration, define directly

$$
T_0=0,\qquad T_n=\inf\{t\geq T_{n-1}+1:\Theta_t=0\}.
$$

The logarithmic lift makes $\Theta$ a continuous adapted process. Hitting a closed set after a stopping time is a stopping time under the usual filtration conditions, and the unbounded zero set proves inductively that each $T_n$ is finite almost surely. Since $T_n\geq T_{n-1}+1$, the sequence tends to infinity, and continuity gives

$$
\boxed{\zeta^2_{\tau(T_n)}=\Theta_{T_n}=0\quad\text{for every }n.}
$$

Geometrically, the Brownian path returns to the positive real ray at arbitrarily late times with **zero net unwrapped winding angle** about the origin. The assertion is stronger than principal argument zero, which also allows any integer number of completed turns.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
