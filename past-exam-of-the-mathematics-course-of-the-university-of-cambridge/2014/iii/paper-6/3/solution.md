<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) says that a positive [linear functional](../../../../../linear-functional.md) on $C(K)$ has the form $f\mapsto\int_Kf\,d\nu$ for a unique finite positive [regular Borel measure](../../../../../regular-borel-measure.md) $\nu$, with [norm](../../../../../norm.md) $\nu(K)$. Its complex form says that every bounded complex [linear functional](../../../../../linear-functional.md) is represented by a unique finite regular [complex measure](../../../../../complex-measure.md) $\mu$, and

$$
\boxed{C(K)^*\cong M(K),\qquad L_\mu(f)=\int_Kf\,d\mu,\qquad\|L_\mu\|=|\mu|(K).}
$$

The extension from positive to arbitrary [linear functionals](../../../../../linear-functional.md) follows by positive/negative decomposition of real [linear functionals](../../../../../linear-functional.md) and then real/imaginary decomposition. The last quantity is the [total variation norm of a measure](../../../../../total-variation-norm-of-a-measure.md), so this identifies the dual isometrically.

An [extreme point](../../../../../extreme-point.md) $e$ of a [convex set](../../../../../convex-set.md) $C$ cannot be written as $e=ta+(1-t)b$ with $0<t<1$ and distinct $a,b\in C$. The [Krein-Milman theorem](../../../../../krein-milman-theorem.md), applied with the underlying real locally convex [weak-star topology](../../../../../weak-star-topology.md), states

$$
\boxed{C=\overline{\operatorname{conv}(\operatorname{ext}C)}^{\,w^*},\qquad\operatorname{ext}C\neq\varnothing.}
$$

We next prove [Milman's converse to the Krein-Milman theorem](../../../../../milman-s-converse-to-the-krein-milman-theorem.md). Suppose an [extreme point](../../../../../extreme-point.md) $e$ were outside the weak-star closure of $S$. A basic weak-star neighborhood of $e$ disjoint from $S$ uses finitely many real coordinates: real and imaginary parts of evaluations at elements of $X$. Its complement is the union of finitely many closed half-spaces

$$
\ell_j(c)-\ell_j(e)\geq\varepsilon_j\quad\text{or}\quad\ell_j(c)-\ell_j(e)\leq-\varepsilon_j.
$$

Intersect these with $C$, discard empty intersections, and call the resulting compact [convex sets](../../../../../convex-set.md) $C_1,\ldots,C_m$. They cover $S$, and none contains $e$.

The [convex hull](../../../../../convex-hull.md) of their union is compact. Every point in it can be written $\sum_{i=1}^mt_ic_i$ with $(t_i)$ in the finite simplex and $c_i\in C_i$, by combining terms from the same [convex set](../../../../../convex-set.md). The map from the simplex times $\prod_iC_i$ to that sum is weak-star continuous, so its image is compact and closed. It therefore contains $\overline{\operatorname{conv}S}^{\,w^*}=C$, in particular $e$. But extremality forces every $c_i$ having a positive coefficient in a representation of $e$ to equal $e$, contradicting $e\notin C_i$. Hence

$$
\boxed{\operatorname{ext}C\subseteq\overline S^{\,w^*}.}
$$

Assume $K\neq\varnothing$. We claim that the [extreme points of the dual unit ball of C(K)](../../../../../extreme-points-of-the-dual-unit-ball-of-c-k.md) are

$$
\boxed{\operatorname{ext}B_{C(K)^*}=\{\alpha\delta_t:t\in K,\ |\alpha|=1\}.}
$$

A measure of [norm](../../../../../norm.md) less than one is not extreme, since it admits a small nonzero perturbation $\pm\eta\delta_t$ within the ball. For a measure $\mu$ of [norm](../../../../../norm.md) one, suppose $|\mu|$ is not a point mass. There is a Borel set $E$ with $0<a=|\mu|(E)<1$: if the [measure support](../../../../../support-of-a-measure.md) has two points, choose disjoint neighborhoods of positive mass; a regular probability measure supported at just one point is the corresponding point mass. Then

$$
\mu=a\frac{\mu|_E}{a}+(1-a)\frac{\mu|_{K\setminus E}}{1-a}
$$

is a convex combination of distinct norm-one measures. Thus an extreme measure must have variation concentrated at one point, and must be $\alpha\delta_t$ with $|\alpha|=1$.

Conversely, if $\alpha\delta_t=(\nu+\eta)/2$ with $\|\nu\|,\|\eta\|\leq1$, then

$$
1=\left|\frac{\nu(\{t\})+\eta(\{t\})}{2}\right|\leq\frac{|\nu(\{t\})|+|\eta(\{t\})|}{2}\leq1.
$$

Equality throughout forces both measures to have all their variation at $t$, and forces their phases to be $\alpha$. Hence $\nu=\eta=\alpha\delta_t$, proving extremality. If $K=\varnothing$, the dual ball is $\{0\}$ and its sole [extreme point](../../../../../extreme-point.md) is $0$.

Every finite [Borel measure](../../../../../borel-measure.md) on $[0,1]$ is regular, so the given $\mu$ belongs to the dual [unit ball](../../../../../unit-ball.md) of $C[0,1]$. Apply [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) and [Krein-Milman theorem](../../../../../krein-milman-theorem.md) to that ball. It is the weak-star closed [convex hull](../../../../../convex-hull.md) of these phased point masses. The [unit ball](../../../../../unit-ball.md) of the finite-dimensional [vector subspace](../../../../../vector-subspace.md) $F$ is [norm](../../../../../norm.md) compact. Choose a finite $\varepsilon/4$-net $f_1,\ldots,f_m$ in it. There is a convex combination

$$
\nu=\sum_{i=1}^Na_i\alpha_i\delta_{w_i},\qquad a_i\geq0,\quad\sum_i a_i=1,\quad|\alpha_i|=1,
$$

whose integrals differ from those of $\mu$ by less than $\varepsilon/2$ on every $f_j$. Put $t_i=a_i\alpha_i$. Then **$\sum_i|t_i|=1$** and $\|\nu\|\leq1$. For any $f$ in the [unit ball](../../../../../unit-ball.md) of $F$, choose $f_j$ with $\|f-f_j\|<\varepsilon/4$. The [linear functional](../../../../../linear-functional.md) $L_\mu-L_\nu$ has [norm](../../../../../norm.md) at most two, so

$$
\left|\int f\,d\mu-\sum_it_if(w_i)\right|<\frac\varepsilon2+2\frac\varepsilon4=\varepsilon.
$$

Scaling yields the requested estimate for every $f\in F$. This is [atomic approximation on finite-dimensional spaces of continuous functions](../../../../../atomic-approximation-on-finite-dimensional-spaces-of-continuous-functions.md). Repeated nodes are allowed: keeping their individual terms preserves the exact sum of coefficient magnitudes even if their phases cancel. If $F=\{0\}$, one point with coefficient one suffices.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
