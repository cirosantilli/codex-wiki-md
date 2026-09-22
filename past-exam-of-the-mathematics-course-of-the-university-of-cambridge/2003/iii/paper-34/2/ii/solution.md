<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For unit resource requirements, treat the resource-blocking events as approximately independent. Let $B_j$ be the approximate blocking probability at resource $j$. Screening class-$r$ traffic by every resource other than $j$ produces the [reduced-load approximation](../../../../../../reduced-load-approximation.md)

$$
a_j=\sum_{r:j\in r}\alpha_r\prod_{k\in r\setminus\{j\}}(1-B_k),
\qquad
\boxed{B_j=E(a_j,C_j).}
$$

The modeled resource is excluded from its own screening product. For general integer requirements, the standard generalized approximation is $a_j=(1-B_j)^{-1}\sum_r A_{jr}\alpha_r\prod_k(1-B_k)^{A_{kr}}$; in the unit-requirement case this reduces to the displayed formula. The approximate route acceptance is $\prod_j(1-B_j)^{A_{jr}}$. The [independence](../../../../../../independent-random-variables.md) used here is an approximation to the correlated exact [stationary distribution](../../../../../../stationary-distribution.md), not an extra property of that law.

Here is a proof of fixed-routing existence and uniqueness. Suppose first that every retained capacity $C_j$ is a positive integer. Links of zero capacity permanently reject their routes and can be removed. If $K$ has the [upper-truncated Poisson distribution](../../../../../../upper-truncated-poisson-distribution.md) with parameter $a$, its mean is

$$
m_C(a)=a[1-E(a,C)],\qquad m_C'(a)=\frac{\operatorname{Var}_a(K)}a>0\quad(a>0).
$$

The [derivative](../../../../../../derivative.md) follows by differentiating the normalized weights: $dP(K=k)/da=P(K=k)(k-m_C(a))/a$. The probability at the upper endpoint similarly gives

$$
\frac{d}{da}E(a,C)=\frac{E(a,C)}a[C-m_C(a)]>0.
$$

Thus $E(\cdot,C)$ increases from zero to one, while $m_C$ increases from zero to $C$. This is the [monotonicity of the Erlang blocking probability](../../../../../../monotonicity-of-the-erlang-blocking-probability.md).

Set $y_j=-\log(1-B_j)$. For $y\geq0$ define

$$
u_j(y)=e^{-y}E(\cdot,C_j)^{-1}(1-e^{-y}).
$$

Here the inverse is with respect to [offered load](../../../../../../offered-traffic.md), and the value at zero is zero. This function is the carried load evaluated at the inverse blocking coordinate, so it is continuous and strictly increasing, with limit $C_j$ as $y\to\infty$. Consider the [convex potential for the Erlang fixed point](../../../../../../convex-potential-for-the-erlang-fixed-point.md)

$$
F(y)=\sum_r\alpha_r\exp\left(-\sum_jA_{jr}y_j\right)
+\sum_j\int_0^{y_j}u_j(z)\,dz.
$$

Each exponential of a [linear function](../../../../../../linear-function.md) is convex. Each integral is [strictly convex](../../../../../../strictly-convex-function.md) because its [derivative](../../../../../../derivative.md) $u_j$ is strictly increasing. Their sum is [strictly convex](../../../../../../strictly-convex-function.md) on the [nonnegative orthant](../../../../../../nonnegative-orthant.md). It is also coercive: for large $y_j$, $u_j(y_j)$ is bounded below by a positive constant, so the integral grows without bound; the other terms are nonnegative. Hence $F$ attains a unique minimum.

At a positive coordinate, the [first-order condition](../../../../../../first-order-optimality-condition.md) is

$$
u_j(y_j)=\sum_r A_{jr}\alpha_r
\exp\left(-\sum_k A_{kr}y_k\right).
$$

At $y_j=0$, the [derivative](../../../../../../derivative.md) equals minus the right-hand side and is nonpositive. A boundary minimum can therefore occur there only when that load is zero, in which case the [derivative](../../../../../../derivative.md) is zero and the same equation holds. Since $1-B_j=e^{-y_j}$, division by this positive acceptance probability makes the [first-order condition](../../../../../../first-order-optimality-condition.md) precisely the reduced-load equations above. Conversely every fixed point is such a minimum. Thus **[fixed routing](../../../../../../fixed-routing.md) has exactly one [Erlang fixed point](../../../../../../erlang-fixed-point-approximation.md)**, including zero blocking at unused resources. The proof does not rely on a potentially nonconvergent simultaneous substitution algorithm.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
