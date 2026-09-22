<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [prescribed-speed time parametrization of a curve](../../../../../../prescribed-speed-time-parametrization-of-a-curve.md). On a regular part traversed in increasing $u$, let $q(u)=\|F'(u)\|>0$ and assume the prescribed [speed](../../../../../../speed.md) $v(F(u))$ is positive. The chain rule for [velocity](../../../../../../velocity.md) gives

$$
\left\|{dF\over dt}\right\|=q(u){du\over dt}=v(F(u)),\qquad \boxed{{du\over dt}={v(F(u))\over q(u)}}.
$$

Integrate this scalar [ordinary differential equation](../../../../../../ordinary-differential-equation.md) with an adaptive [Runge-Kutta method](../../../../../../runge-kutta-method.md), arranging output at the exact times $t_k=t_0+k\Delta t$. Evaluate $P_k=F(u(t_k))$. Internal integration steps may be shorter than $\Delta t$; output interpolation must meet the same error tolerance, so variable numerical steps do not create variable frame times.

An equivalent implementation precomputes

$$
t(u)-t(0)=\int_0^u{\|F'(\xi)\|\over v(F(\xi))}\,d\xi
$$

by adaptive [numerical integration](../../../../../../numerical-integration.md). This function is strictly increasing. Bracket each $t_k$ in the table and invert using safeguarded [Newton method](../../../../../../newton-s-method-in-optimization.md) or [interval bisection](../../../../../../interval-bisection.md); monotonicity makes each solution unique. Stop at $u=1$, with a shorter final time interval if the total travel time is not a multiple of $\Delta t$. This accounts for changes in both the curve's parameter [speed](../../../../../../speed.md) and the physical [speed](../../../../../../speed.md), unlike equal increments in $u$.

If the specified [speed](../../../../../../speed.md) vanishes, examine the reciprocal-speed integral at that event. It may diverge, giving asymptotic approach, or be integrable, giving arrival in finite time. A scalar [speed](../../../../../../speed.md) does not determine whether motion reverses or how it resumes after stopping; such behavior needs the physical dynamics or a chosen continuation. The positive-speed formula applies between these events, with the direction changed if the traversal reverses.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
