<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [two-state ion-channel gating](../../../../two-state-ion-channel-gating.md), let $\alpha_n(V)$ and $\beta_n(V)$ be the rates of entering and leaving the permissive state. Gain minus loss gives

$$
\dot n=\alpha_n(1-n)-\beta_n n=(\alpha_n+\beta_n)(n_\infty-n),\qquad
n_\infty=\frac{\alpha_n}{\alpha_n+\beta_n},\quad
\tau_n=\frac1{\alpha_n+\beta_n}.
$$

At fixed [membrane potential](../../../../membrane-potential-split.md), these coefficients are constant. The deviation $w=n-n_\infty$ obeys $\dot w=-w/\tau_n$, so the initial condition $n(0)=n_0$ yields

$$
\boxed{n(t)=n_\infty-(n_\infty-n_0)e^{-t/\tau_n}.}
$$

This approaches the fixed-voltage limit monotonically and stays between $n_0$ and $n_\infty$, as a valid [probability](../../../../probability.md) must.

**Convention qualification:** the displayed single [exponential function](../../../../exponential-function.md) describes a voltage-clamp step, not an arbitrary time-dependent [action potential](../../../../action-potential.md). For example, a second imposed voltage step changes both coefficients and requires a new exponential segment. For general $V(t)$ the integrating-factor solution is $n(t)=e^{-A(t)}[n_0+\int_0^t\alpha_n(V(s))e^{A(s)}\,ds]$, with $A(t)=\int_0^t[\alpha_n(V(s))+\beta_n(V(s))]\,ds$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
