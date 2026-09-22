# Conic primal-dual gap

↑ **Parent:** [Conic dual problem](conic-dual-problem.md)

For a [feasible point](feasible-point.md) $x$ and a feasible [dual variable](dual-variable.md) $y$, [weak duality](weak-duality.md) follows from one identity:

$$
g=c^Tx-b^Ty=(Ax-b)^Ty\geq0.
$$

The inequality is the defining property of the [dual cone](dual-cone.md). Every feasible pair therefore encloses the optimal [objective function](objective-function.md) value:

$$
b^Ty\leq d_*\leq p_*\leq c^Tx.
$$

Both optima are finite when such a pair exists. Consequently,

$$
0\leq c^Tx-p_*\leq g,\qquad 0\leq d_*-b^Ty\leq g.
$$

These are absolute cost bounds, rather than bounds on distance to an optimizing [vector](vector.md). Zero gap certifies both optima immediately. A small positive gap bounds the remaining improvement even if no [strong duality](strong-duality.md) theorem has been invoked.

For the [nonnegative-orthant optimality certificate](nonnegative-orthant-optimality-certificate.md) example, $x=(2.9,0.2)^T$ is feasible and costs $3.3$. Pairing it with $y=(0,1,1)^T$ gives $g=0.3$, so its cost exceeds the optimum by at most $0.3$. Here the optimum is known to be $3$, and the bound is exact. Pairing the same $x$ with the weaker $r=1/2$ certificate gives $g=1.8$: a valid but less informative guarantee.

The identity assumes exact primal and dual feasibility. With a dual [linear-system residual](linear-system-residual.md) $r_d=c-A^Ty$, it becomes

$$
c^Tx-b^Ty=(Ax-b)^Ty+x^Tr_d.
$$

The second term has no guaranteed sign. Checking only a small [linear-system residual](linear-system-residual.md) and the cone [dot product](dot-product.md) is insufficient when $\|x\|_2$ is large; a separate bound $|x^Tr_d|\leq\|x\|_2\|r_d\|_2$ follows from the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). Approximate cone membership likewise needs a quantified correction before claiming a certificate.

For an exact arithmetic example, minimize $x$ subject to $x\geq10^9$. The point $x=10^9$ is optimal. A proposed multiplier $y=1+10^{-9}$ is nonnegative and gives zero cone [dot product](dot-product.md) because the slack is zero, but violates $A^Ty=c$ by $10^{-9}$. Its purported lower bound is $10^9+1$, exceeding the optimum. The missing term $x^Tr_d=-1$ explains the failure.

## ↑ Ancestors (7)

1. [Conic dual problem](conic-dual-problem.md)
2. [Conic optimization](conic-optimization.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
