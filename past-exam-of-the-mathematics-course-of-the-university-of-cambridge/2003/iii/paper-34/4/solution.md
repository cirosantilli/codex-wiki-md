<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For active-route per-flow rates $x_r>0$, feasibility means $\sum_{r:j\in r}n_rx_r\leq C_j$ for every resource. The defining condition for a [proportionally fair allocation](../../../../../proportional-fairness.md) is that every feasible alternative $\widetilde x$ satisfies

$$
\sum_{r:n_r>0}n_r\frac{\widetilde x_r-x_r}{x_r}\leq0.
$$

This is equivalent to maximizing [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md) $\sum_{r:n_r>0}n_r\log x_r$ over the feasible set. Its [gradient](../../../../../gradient.md) is $(n_r/x_r)$, so the displayed inequality is precisely the [first-order condition](../../../../../first-order-optimality-condition.md) for this [concave function](../../../../../concave-function.md). [Strict concavity](../../../../../strict-concavity.md) gives unique active-flow rates. Routes with $n_r=0$ have no utility term or actual per-flow rate to determine; set their aggregate service to zero. This is the [inactive routes in proportional fairness](../../../../../inactive-routes-in-proportional-fairness.md) convention.

Abbreviate the route populations as $n_1,n_2,n_3,n_4$ in cyclic order and let $z_r=n_rx_r$ denote aggregate route service. The resource constraints are

$$
z_1+z_4\leq1,\quad z_1+z_2\leq1,\quad
z_2+z_3\leq1,\quad z_3+z_4\leq1.
$$

Equivalently, $\max(z_1,z_3)+\max(z_2,z_4)\leq1$. Fix these two maxima as $u,v$. Because utility is increasing in each active allocation, every active odd route attains $u$ and every active even route attains $v$. Dropping terms constant in the populations, the objective becomes

$$
P\log u+Q\log v,\qquad
P=n_1+n_3,\quad Q=n_2+n_4,\quad M=P+Q.
$$

If both groups are nonempty, the maximum has $u+v=1$ and [derivative](../../../../../derivative.md) $P/u-Q/(1-u)=0$, giving $u=P/M,v=Q/M$. If one group is empty, every route in the other group gets aggregate service one. For $M>0$, all cases are summarized, on active routes, by

$$
\boxed{x_r=\begin{cases}
P/(Mn_r),&r=1,3,\ n_r>0,\\
Q/(Mn_r),&r=2,4,\ n_r>0.
\end{cases}}
$$

At $M=0$ there are no flows and all aggregate services are zero. In particular $n_1x_1=(n_1+n_3)/M$ whenever $n_1>0$, as printed in the PDF. The per-flow rate is not generally $1/M$: opposite routes can use the same resource capacities in parallel.

An exponential document size with parameter $\mu_r$ has completion hazard $\mu_rx_r$ when a flow is served at rate $x_r$. Summing over its $n_r$ flows gives the [transition rates](../../../../../transition-intensity.md)

$$
\boxed{q(n,n+e_r)=\nu_r,\qquad
q(n,n-e_r)=\mu_rn_rx_r(n)\quad(n_r>0).}
$$

Thus an active odd route departs at rate $\mu_rP/M$, and an active even route at rate $\mu_rQ/M$. An empty route has departure rate zero even if its opposite route is populated.

Put $\alpha_r=\nu_r/\mu_r$ and

$$
\Phi(n)=\binom{M}{P},\qquad \Phi(0)=1.
$$

For an active odd route and an active even route respectively,

$$
\frac{\Phi(n-e_r)}{\Phi(n)}=\frac PM,
\qquad
\frac{\Phi(n-e_r)}{\Phi(n)}=\frac QM.
$$

Hence aggregate service is the neighboring-state ratio of this [balance function of a flow-level network](../../../../../balance-function-of-a-flow-level-network.md). Consider weights $w(n)=\Phi(n)\prod_r\alpha_r^{n_r}$. For every birth edge,

$$
w(n+e_r)\mu_r\frac{\Phi(n)}{\Phi(n+e_r)}=w(n)\nu_r.
$$

These are [detailed balance equations](../../../../../detailed-balance.md). The total departure rate is bounded by $\sum_r\mu_r$ and total arrival rate by $\sum_r\nu_r$, so the process is nonexplosive. Provided the normalizing sum is finite, its [stationary distribution](../../../../../stationary-distribution.md) is therefore

$$
\boxed{\pi(n)=B^{-1}\binom{n_1+n_2+n_3+n_4}{n_1+n_3}
\prod_{r=1}^4\left(\frac{\nu_r}{\mu_r}\right)^{n_r}.}
$$

The large parentheses in the original PDF represent a [binomial coefficient](../../../../../binomial-coefficient.md), not a ratio. The verified adjacent-state ratios explain why that distinction matters.

The required stability condition can be established directly from the normalizing sum. Set $a=\alpha_1,c=\alpha_3,b=\alpha_2,d=\alpha_4$, and $h_p(a,c)=\sum_{i=0}^pa^ic^{p-i}$. Grouping opposite-route counts gives

$$
B=\sum_{p,q\geq0}\binom{p+q}{p}h_p(a,c)h_q(b,d).
$$

If $A_* =\max(a,c)$ and $B_* =\max(b,d)$, then $A_*^p\leq h_p\leq(p+1)A_*^p$, with the same bounds for the other group. Restriction to the routes attaining the maxima bounds $B$ below by $\sum_m(A_*+B_*)^m$. If $A_*+B_*<1$, the upper bound is at most $\sum_m(m+1)^2(A_*+B_*)^m$, which converges. Thus

$$
\boxed{B<\infty\iff\max(\alpha_1,\alpha_3)+\max(\alpha_2,\alpha_4)<1.}
$$

Equivalently every resource's [offered load](../../../../../offered-traffic.md) is strictly below its unit capacity. With positive arrival rates the irreducible chain then has the unique stationary probability distribution above. Without this condition the weights remain an invariant measure but are not normalizable; the question's probability-distribution claim implicitly needs this hypothesis.

For completeness, the [normalizing constant](../../../../../normalizing-constant.md) has the [four-cycle partition function](../../../../../four-cycle-partition-function.md) expression

$$
B=\frac{(1-a)(1-b)(1-c)(1-d)-abcd}
{(1-a-b)(1-a-d)(1-c-b)(1-c-d)}.
$$

To derive it when $a\ne c$ and $b\ne d$, substitute $h_p=(a^{p+1}-c^{p+1})/(a-c)$ into the double sum and use $\sum_{p,q}\binom{p+q}{p}u^pv^q=(1-u-v)^{-1}$. The resulting expression is

$$
\frac1{(a-c)(b-d)}\left[
\frac{ab}{1-a-b}-\frac{ad}{1-a-d}-\frac{cb}{1-c-b}+\frac{cd}{1-c-d}\right],
$$

which simplifies to the displayed formula. [Continuity](../../../../../continuous-function.md) within the stability region covers equal opposite loads and zero loads.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
