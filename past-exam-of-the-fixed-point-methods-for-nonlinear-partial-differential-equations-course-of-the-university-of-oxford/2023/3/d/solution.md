<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the [functional](../../../../functional.md)

$$
\boxed{J(u)=\int_\Omega\left(\frac14|\nabla u|^4+\frac18|u|^8-fu\right)dx,
\qquad u\in W_0^{1,4}(\Omega).}
$$

The factor $1/8$ is essential: the [derivative](../../../../derivative.md) of $|s|^8/8=s^8/8$ is $s^7$, while the [gradient](../../../../gradient.md) with respect to $\xi$ of $|\xi|^4/4$ is $|\xi|^2\xi$. As in part (c), finite polynomial expansions and [Hölder's inequality](../../../../holder-s-inequality.md) justify differentiation along every direction $v\in X$, giving $DJ(u)[v]=\langle A(u),v\rangle$.

We prove the global and strict minimum directly. The [strictly convex functions](../../../../strictly-convex-function.md) $\Phi(\xi)=|\xi|^4/4$ and $\Psi(s)=|s|^8/8$ satisfy their tangent inequalities

$$
\Phi(\eta)\geq\Phi(\xi)+|\xi|^2\xi\cdot(\eta-\xi),
\qquad
\Psi(t)\geq\Psi(s)+s^7(t-s),
$$

with strict inequality when the respective arguments differ. For example, strict [convexity](../../../../convex-function.md) of $\Phi$ follows from strict [operator monotonicity](../../../../operator-monotonicity.md) of its [gradient](../../../../gradient.md), proved by the midpoint identity in part (b)(iii); strict [convexity](../../../../convex-function.md) of $\Psi$ follows because its [derivative](../../../../derivative.md) $s^7$ is strictly increasing.

Apply these inequalities pointwise to $\nabla u_*,\nabla v$ and $u_*,v$, then integrate. The [weak formulation](../../../../weak-formulation.md) at $u_*$ with [test function](../../../../test-function.md) $v-u_*$ gives

$$
J(v)-J(u_*)\geq\langle A(u_*),v-u_*\rangle=0.
$$

If $v\ne u_*$ in $X$, the [Poincaré inequality](../../../../poincare-inequality.md) implies $\nabla v\ne\nabla u_*$ on a set of positive [Lebesgue measure](../../../../lebesgue-measure.md). The first tangent inequality is strict on that set and the second is nonnegative everywhere. Their integrable remainders therefore have strictly positive total [integral](../../../../integral-split.md). Hence

$$
\boxed{J(v)>J(u_*)\quad\text{for every }v\in X\setminus\{u_*\}.}
$$

Thus $u_*$ is the unique global [minimizer](../../../../global-minimizer.md) of $J$. Conversely, every [minimizer](../../../../global-minimizer.md) has zero directional [derivative](../../../../derivative.md) in every direction and so satisfies $A(u)=0$, which also identifies it with the unique [weak solution](../../../../weak-solution.md) from part (c).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
