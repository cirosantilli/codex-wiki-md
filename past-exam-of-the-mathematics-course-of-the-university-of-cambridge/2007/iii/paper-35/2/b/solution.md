<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume each link delay $\ell_e$ is continuous and nondecreasing. Define the [Beckmann potential](../../../../../../beckmann-potential.md) on feasible route flows by

$$
\Psi(f)=\sum_e\int_0^{(Af)_e}\ell_e(u)\,du.
$$

The integral of a nondecreasing function is [convex](../../../../../../convex-function.md), so $\Psi$ is a [convex function](../../../../../../convex-function.md). The [chain rule](../../../../../../chain-rule.md) gives

$$
\frac{\partial\Psi}{\partial f_p}=L_p(f).
$$

At a minimum, move a small amount of flow from a used route $p$ to any other route $q$ for the same source-sink pair. This is a feasible direction, and its one-sided derivative is $L_q-L_p\geq0$. Thus every used route has minimum cost, establishing the [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md) conditions.

Conversely, if $f$ satisfies the [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md) conditions, then for any feasible $g$,

$$
\nabla\Psi(f)\cdot(g-f)=\sum_k\sum_{p\in\mathcal P_k}L_p(f)(g_p-f_p)\geq\sum_k\lambda_k\sum_{p\in\mathcal P_k}(g_p-f_p)=0.
$$

Here $\sum_pL_pf_p=\lambda_kd_k$ on each pair, whereas $\sum_pL_pg_p\geq\lambda_kd_k$. The supporting inequality for a [convex function](../../../../../../convex-function.md) then gives $\Psi(g)\geq\Psi(f)$. Therefore

$$
\boxed{\text{Wardrop equilibria are precisely the minimizers of the Beckmann potential.}}
$$

The feasible route-flow set is compact, and the [Beckmann potential](../../../../../../beckmann-potential.md) is continuous, so a minimizer exists. If each $\ell_e$ is strictly increasing, the potential is strictly convex as a function of link loads. Two minimizers with distinct link-load vectors would have a midpoint with strictly smaller potential, a contradiction. Thus equilibrium link loads are unique in this case; [route-flow nonuniqueness at a Wardrop equilibrium](../../../../../../route-flow-nonuniqueness-at-a-wardrop-equilibrium.md) can still occur because different route decompositions can have the same link loads.

The optimization of selfish route choice must be distinguished from the minimization of total travel time

$$
D(f)=\sum_p f_pL_p(f)=\sum_ev_e\ell_e(v_e).
$$

For differentiable delays, the marginal social cost on link $e$ is $\ell_e(v_e)+v_e\ell_e'(v_e)$, rather than just $\ell_e(v_e)$. The [marginal external cost toll](../../../../../../marginal-external-cost-toll.md) $\tau_e(v_e)=v_e\ell_e'(v_e)$ makes each traveler's perceived link cost equal to this derivative. If $D$ is [convex](../../../../../../convex-function.md), the tolled [Wardrop equilibria](../../../../../../wardrop-equilibrium.md) minimize $D$: the corresponding [Beckmann potential](../../../../../../beckmann-potential.md) is exactly $D$, up to its zero reference value. Convexity of $D$ is an additional assumption and does not follow merely from nondecreasing delays.

An elastic-demand extension assigns pair $k$ an [inverse demand function](../../../../../../inverse-demand-function.md) $P_k(d_k)$ and allows demand to vary. Subtracting $\sum_k\int_0^{d_k}P_k(u)\,du$ from the [Beckmann potential](../../../../../../beckmann-potential.md) produces the optimization formulation: its marginal condition equates minimum route delay with marginal willingness to travel on positive-demand pairs. With decreasing inverse demands, the subtracted utility is concave and the resulting objective remains convex. This explains why both fixed-demand route choice and an [elastic-demand Wardrop equilibrium](../../../../../../elastic-demand-wardrop-equilibrium.md) fit a common optimization framework.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
