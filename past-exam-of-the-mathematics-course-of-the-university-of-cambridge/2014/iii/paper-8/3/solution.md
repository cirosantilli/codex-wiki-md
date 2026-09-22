<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [transport plan](../../../../../transport-plan.md) is a [Borel probability measure](../../../../../borel-probability-measure.md) on $X\times Y$ with marginals $\mu,\nu$. It is [c-cyclically monotone](../../../../../c-cyclical-monotonicity.md) when it is concentrated on a set $\Gamma$ such that every finite list $(x_i,y_i)\in\Gamma$ satisfies

$$
\sum_{i=1}^m c(x_i,y_i)\le\sum_{i=1}^m c(x_{i+1},y_i),\qquad x_{m+1}=x_1.
$$

Equivalently, one can allow every permutation of the destinations, since a permutation decomposes into cycles. The word $c$-monotone here means this cyclic condition, not merely a two-point test for an arbitrary cost.

The potential-certificate meaning of the printed “strictly $c$-monotone” is [strong c-monotonicity](../../../../../strong-c-monotonicity.md): there are Borel [functions](../../../../../function-split.md) $u:X\to\mathbb R\cup\{-\infty\}$ and $v:Y\to\mathbb R\cup\{-\infty\}$ such that

$$
\boxed{u(x)+v(y)\le c(x,y)\text{ everywhere},\qquad u(x)+v(y)=c(x,y)\quad\pi\text{-almost everywhere}.}
$$

The [functions](../../../../../function-split.md) are finite on full marginal-[measure](../../../../../measure.md) sets. This is a certificate by [Kantorovich potentials](../../../../../kantorovich-potential.md), not literal strict inequality in every nonidentity cycle. Such a literal interpretation could not satisfy the requested implication, already for $c=0$.

Here is a direct [transport potential path construction](../../../../../transport-potential-path-construction.md). Since $c$ is finite and continuous, the closure of a cyclically monotone set remains cyclically monotone. We may therefore use the closed support $\Gamma$ of $\pi$ and choose a countable dense subset $\Gamma_0$, containing an anchor $(x_0,y_0)$. For a chain $(x_j,y_j)\in\Gamma_0$, $j=0,\ldots,m$, starting at that anchor, define

$$
L_m(z)=\sum_{j=0}^{m-1}\bigl[c(x_{j+1},y_j)-c(x_j,y_j)\bigr]
+c(z,y_m)-c(x_m,y_m),\qquad
u(z)=\inf_{m,\,\text{chains}}L_m(z).
$$

The infimum is over countably many continuous [functions](../../../../../function-split.md), so $u$ is [upper semicontinuous](../../../../../upper-semicontinuity.md) and Borel, and never $+\infty$ because the zero-length chain is available. Cyclical monotonicity applied to a chain closing at the anchor gives $u(x_0)=0$. If $(x,y)\in\Gamma$, closing a chain through this extra pair gives

$$
L_m(x)\ge c(x,y)-c(x_0,y),
$$

so $u(x)$ is finite on the first projection of $\Gamma$.

Append the pair $(x,y)$ to a nearly minimizing chain ending at $x$. If the pair is outside $\Gamma_0$, approximate it by pairs in $\Gamma_0$ and use continuity of the finitely many costs. This gives, for every $z$,

$$
u(z)\le u(x)+c(z,y)-c(x,y)\qquad ((x,y)\in\Gamma).
$$

Now put

$$
v(y)=\inf_{z:\,u(z)>-\infty}\bigl[c(z,y)-u(z)\bigr].
$$

It is again an infimum of continuous [functions](../../../../../function-split.md) of $y$, and therefore [upper semicontinuous](../../../../../upper-semicontinuity.md) and Borel. The anchor bounds it above by $c(x_0,y)$. Feasibility $u(z)+v(y)\le c(z,y)$ is immediate. For $(x,y)\in\Gamma$, the preceding chain inequality gives $v(y)\ge c(x,y)-u(x)$, while testing $z=x$ gives the opposite inequality. Hence equality holds on $\Gamma$, and $v$ is finite on its second projection. This proves **cyclical monotonicity implies the potential certificate**.

To deduce optimality, we must not subtract possibly infinite marginal integrals. Use the [symmetric clipping proof of transport optimality](../../../../../symmetric-clipping-proof-of-transport-optimality.md): let $u_n=\max(-n,\min(u,n))$ and similarly $v_n$. Because $c\ge0$, simultaneous clipping preserves the feasible inequality

$$
u_n(x)+v_n(y)\le\max\{u(x)+v(y),0\}\le c(x,y).
$$

For any competitor $\pi'$ with the same marginals, boundedness gives

$$
\int(u_n+v_n)\,d\pi
=\int u_n\,d\mu+\int v_n\,d\nu
=\int(u_n+v_n)\,d\pi'\le\int c\,d\pi'.
$$

On the full-[measure](../../../../../measure.md) equality set for $\pi$, $u+v=c\ge0$. There the clipped sums are nonnegative and increase to $c$: when the two signs differ, their large equal clipping levels initially cancel, then the sum increases to the nonnegative original sum. Thus the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) gives

$$
\boxed{\int c\,d\pi\le\int c\,d\pi'\quad\text{for every competitor}.}
$$

This proves optimality even if the eventual integral is infinite. Conversely, a potential certificate implies the cyclic inequalities by summing and cancelling the potentials on its full-[measure](../../../../../measure.md) equality set.

**The converse from optimality is true for finite-cost optimal plans.** To see this, suppose points in the support violate a finite cyclic inequality by a positive amount. Continuity supplies product neighborhoods of those points on which every selected tuple still violates it, with all involved costs bounded. Normalize the restrictions of $\pi$ to these neighborhoods to [probability measures](../../../../../probability-measure.md) $\alpha_i$, with marginals $\mu_i,\nu_i$. Subtract a sufficiently small common multiple of $\sum_i\alpha_i$ and add the same multiple of $\sum_i\mu_{i+1}\otimes\nu_i$. Positivity is ensured by choosing the multiple at most $\min_i\pi(U_i)/m$, even if neighborhoods overlap. Both marginals are unchanged, but integration of the strict cyclic improvement over the product of the $\alpha_i$ decreases the finite total cost. This contradicts optimality, so the support is cyclically monotone.

Without a finite-value hypothesis, the unrestricted converse is false. On the discrete Polish spaces $X=Y=\mathbb N$, take $\mu(n)=\nu(n)=C/n^2$ and

$$
c(m,n)=m+n+1_{\{m=n\}}.
$$

This is finite, continuous and nonnegative, yet every coupling has infinite cost because its marginals have infinite first moments. The diagonal plan is therefore an extended-value minimizer. Its support is not cyclically monotone: two distinct diagonal pairs cost $2m+2n+2$, while swapping their destinations costs $2m+2n$. Thus **under the literal printed hypotheses, optimality alone need not imply $c$-monotonicity; the usual finite-cost converse needs that qualification**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
