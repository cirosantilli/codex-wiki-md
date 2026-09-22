<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The measurable structure of an [exchange economy](../../../../../../exchange-economy.md) includes measurability of consumers' [preference relations](../../../../../../preference-relation.md): in particular, for each rational vector $q$, the set

$$
E_q=\{a:f(a)+q\in\mathbb R_+^L,\ f(a)+q\succ_a f(a)\}
$$

is measurable. Continuity of each individual's [preference relation](../../../../../../preference-relation.md) alone would not imply this across-consumer requirement. We use this usual measurability convention explicitly.

There are only countably many vectors in $\mathbb Q^L$. Remove all the null sets $E_q$ that have zero measure, obtaining

$$
D=A\setminus\bigcup_{\mu(E_q)=0}E_q,\qquad\mu(D)=1.
$$

Let $V=\{q\in\mathbb Q^L:\mu(E_q)>0\}$. Equivalently, $V$ is the union over $a\in D$ of the rational strict-improvement directions available to consumer $a$. This choice of $D$ ensures that a direction available to even one consumer in $D$ is available to a positive-measure group.

We claim that $0\notin\operatorname{co}V$. Otherwise, take finitely many $q_1,\ldots,q_m\in V$ and positive weights $\lambda_i$ with $\sum_i\lambda_i=1$ and $\sum_i\lambda_iq_i=0$. Choose $t>0$ so small that $2t<\min_i\mu(E_{q_i})$. We can choose disjoint measurable sets $F_i\subseteq E_{q_i}$ with $\mu(F_i)=t\lambda_i$. Indeed, after the earlier choices remove at most $t$ mass, the remaining portion of $E_{q_i}$ has mass greater than $t$. The scalar case of the [Lyapunov convexity theorem](../../../../../../lyapunov-convexity-theorem.md), applied to its restricted [atomless measure](../../../../../../non-atomic-measure.md), realizes every mass between zero and its total, including $t\lambda_i$.

Now change $f(a)$ to $f(a)+q_i$ on $F_i$ and leave it unchanged elsewhere. Every changed bundle is a feasible consumption bundle and is strictly preferred by its recipient. This new [consumption allocation](../../../../../../consumption-allocation.md) $g$ remains integrable, and

$$
\int_A(g-f)\,d\mu=\sum_i\mu(F_i)q_i=t\sum_i\lambda_iq_i=0.
$$

Thus $g$ is exactly feasible and improves a group of total mass $t>0$, contradicting [Pareto efficiency](../../../../../../pareto-efficiency.md). Notice that no individual's consumption bundles were averaged: an [atomless measure](../../../../../../non-atomic-measure.md) allows different small cohorts to make different improvements. Individual convexity of the [preference relations](../../../../../../preference-relation.md) is unnecessary.

If $V$ is nonempty, separate its [convex hull](../../../../../../convex-hull.md) from zero using the [supporting hyperplane theorem](../../../../../../supporting-hyperplane-theorem.md). There exists $p\ne0$ with $p\cdot q\geq0$ for every $q\in V$. Only weak separation is needed, so it is harmless if zero belongs to the closure of this [convex hull](../../../../../../convex-hull.md).

Fix any $a\in D$ and any $y\succ_a f(a)$. Completeness and continuity make the strictly preferred set relatively open in $\mathbb R_+^L$. Approximate $y-f(a)$ by rational vectors $q_n$ for which $f(a)+q_n$ is feasible and still strictly preferred. At a zero consumption coordinate, choose the rational approximations from the feasible side. Then $a\in E_{q_n}$ implies $q_n\in V$, and passage to the limit gives $p\cdot(y-f(a))\geq0$. The same full-measure set $D$ works for all such bundles $y$, not merely for each bundle separately.

If $V$ is empty, the same rational approximation argument says that consumers in $D$ have no strictly preferred feasible bundles at all. In that case any nonzero $p$ satisfies the required implication. In either case,

$$
\boxed{(f,p)\text{ is a price quasi-equilibrium with transfers for some }p\ne0.}
$$

To see why transfers cannot simply be omitted, give all consumers endowment $(1,1)$ and [utility function](../../../../../../utility-function-split.md) $u(x_1,x_2)=x_1+x_2$. Allocate $(3/2,3/2)$ to half of them and $(1/2,1/2)$ to the other half. This is [Pareto efficient](../../../../../../pareto-efficiency.md), since any Pareto improvement would increase the integral of utility while aggregate resources fix it. At these interior bundles the support inequalities force $p_1=p_2>0$: directions arbitrarily close to $(1,-1)$ force equality, and strict increases force positivity. The poorer half then receives less wealth than the original endowment supplies and has a cheaper strict improvement within its original budget. The support theorem concerns the redistributed budget, as defined in part (b).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
