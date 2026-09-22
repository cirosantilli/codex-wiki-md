<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The useful [high-density core bound from TOV compactness](../../../../../../../high-density-core-bound-from-tov-compactness.md) follows without choosing the unknown high-density [equation of state](../../../../../../../equation-of-state.md). Let $a$ be the radius at which the decreasing [energy density](../../../../../../../energy-density.md) first reaches $\rho_0$, and put $\mu=m(a)$, $p_0=p(\rho_0)$. The [Tolman–Oppenheimer–Volkoff equation](../../../../../../../tolman-oppenheimer-volkoff-equation.md) gives $p'<0$ away from a nonempty centre; since $dp/d\rho>0$, [energy density](../../../../../../../energy-density.md) decreases outward. Hence

$$
\mu=4\pi\int_0^a\rho(r)r^2\,dr\geq\frac{4\pi}{3}\rho_0a^3.
$$

For the local [stellar compactness](../../../../../../../stellar-compactness.md), if $z\geq0$, $1-z+\sqrt{1+z}\leq2$, since its derivative is $-1+(2\sqrt{1+z})^{-1}<0$. Applying the supplied compactness inequality at the core boundary therefore gives $\mu/a<4/9$. Combining the two bounds yields

$$
\boxed{a<\frac1{\sqrt{3\pi\rho_0}},\qquad\mu<\frac4{9\sqrt{3\pi\rho_0}}.}
$$

The pressure-dependent form further restricts the allowed core-boundary data:

$$
\frac{\mu}{a}<\frac29\left(1-6\pi a^2p_0+\sqrt{1+6\pi a^2p_0}\right).
$$

In particular, positivity of its right side gives $6\pi a^2p_0<3$, so $a^2<1/(2\pi p_0)$ when $p_0>0$. These restrictions depend only on known quantities, not on the [equation of state](../../../../../../../equation-of-state.md) above $\rho_0$.

The intended stellar-mass argument now attaches the known low-density envelope to each admissible pair $(a,\mu)$ with [pressure](../../../../../../../pressure.md) $p_0$. Its [Tolman–Oppenheimer–Volkoff equation](../../../../../../../tolman-oppenheimer-volkoff-equation.md) involves only the known [equation of state](../../../../../../../equation-of-state.md). For a physical low-density envelope with a uniformly bounded [mass](../../../../../../../mass.md) on this bounded set of core data, taking the supremum of the envelope-plus-core masses gives an upper [mass](../../../../../../../mass.md) limit independent of any high-density continuation. Stars with $\rho_c\leq\rho_0$ are also determined entirely by the known [equation of state](../../../../../../../equation-of-state.md). **Unknown dense-core physics cannot evade the displayed core bounds.**

A qualification is necessary for a claim about the entire star: **the printed monotonicity assumptions alone do not guarantee a finite maximum total [mass](../../../../../../../mass.md) for an arbitrary known low-density [equation of state](../../../../../../../equation-of-state.md)**. An explicit [low-density polytropic mass divergence](../../../../../../../low-density-polytropic-mass-divergence.md) occurs for $p=K\rho^{5/4}$ with fixed $K>0$. In the low-density [Newtonian limit](../../../../../../../newtonian-limit.md), this is a [stellar polytrope](../../../../../../../stellar-polytrope.md) of index $n=4$, whose [Lane-Emden equation](../../../../../../../lane-emden-equation.md) has a finite first zero. With $\rho=\rho_c\vartheta^4$ and $r=\ell\xi$, hydrostatic balance fixes

$$
\ell^2=\frac{5K}{4\pi}\rho_c^{-3/4},\qquad M=4\pi\rho_c\ell^3\mu_4\propto\rho_c^{-1/8},\qquad R\propto\rho_c^{-3/8},
$$

where $\mu_4>0$ is the dimensionless [Lane-Emden surface mass constant](../../../../../../../lane-emden-surface-mass-constant.md). Thus $M\to\infty$ as $\rho_c\to0$, although $M/R\propto\rho_c^{1/4}\to0$. The first Lane-Emden zero is simple. The [continuous dependence of an ODE solution on parameters](../../../../../../../continuous-dependence-of-an-ode-solution-on-parameters.md) therefore preserves this finite surface for sufficiently small relativistic parameter. The relativistic correction is controlled by $p_c/\rho_c=K\rho_c^{1/4}\to0$, so the corresponding regular finite-radius [Tolman–Oppenheimer–Volkoff equation](../../../../../../../tolman-oppenheimer-volkoff-equation.md) solutions have the same limiting scalings. They never sample $\rho>\rho_0$, and satisfy the local positivity and monotonicity assumptions in their nonvacuum interiors. This shows exactly why a suitable bounded-envelope hypothesis, or an appropriate restriction to physically stable stellar models, must accompany the intended total-mass conclusion. The compactness inequality supplies a bound on the unknown core, not a bound on the [mass](../../../../../../../mass.md) of every conceivable dilute envelope.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 54](../../../../paper-54-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
