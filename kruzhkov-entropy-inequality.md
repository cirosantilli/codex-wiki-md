# Kruzhkov entropy inequality

↑ **Parent:** [Entropy solution](entropy-solution.md)

For a scalar [conservation law](conservation-law.md) law $u_t+f(u)_x=0$, the Kruzhkov entropy inequalities require

$$
\partial_t|u-c|+\partial_x\bigl(\operatorname{sgn}(u-c)[f(u)-f(c)]\bigr)\le0
$$

in distributions for every real constant $c$, together with the initial trace. This means the integral against every nonnegative compactly supported test function is nonpositive after applying the distributional derivatives. For a smooth solution the entropy balance is an equality away from $u=c$. For a viscous approximation $u_t+f(u)_x=\varepsilon u_{xx}$, smooth convex approximations $\eta$ of $|u-c|$ give $\partial_t\eta(u)+\partial_xq(u)=\varepsilon\partial_{xx}\eta(u)-\varepsilon\eta''(u)u_x^2\le\varepsilon\partial_{xx}\eta(u)$, with $q'=\eta'f'$. Letting the entropy smoothing vanish and then taking a bounded, strongly locally convergent zero-viscosity limit proves the inequality. The discrete entropy inequality of a monotone conservative scheme is its numerical analogue.

## ↑ Ancestors (9)

1. [Entropy solution](entropy-solution.md)
2. [Inviscid Burgers equation](inviscid-burgers-equation.md)
3. [Scalar conservation law](scalar-conservation-law.md)
4. [Transport equation](transport-equation.md)
5. [Partial differential equation](partial-differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/6/solution.md)
