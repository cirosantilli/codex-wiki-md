<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Give $C(G)$, the [space of continuous functions on a compact space](../../../../../space-of-continuous-functions-on-a-compact-space.md), its [uniform norm](../../../../../supremum-norm.md). The [left regular action](../../../../../left-regular-action.md) is $l_gf(x)=f(g^{-1}x)$. The group law gives $l_gl_h=l_{gh}$ and $l_e=I$, and each translation is a linear [isometry](../../../../../isometry.md) because $x\mapsto g^{-1}x$ is a bijection of $G$.

For fixed $f\in C(G)$, the map $(g,x)\mapsto f(g^{-1}x)$ is continuous. Compactness of the $x$-space makes this dependence uniform: for a given $g_0$ and $\varepsilon>0$, continuity gives a [neighbourhood](../../../../../neighbourhood-mathematics.md) of $g_0$ and a [neighbourhood](../../../../../neighbourhood-mathematics.md) of each $x$ on which the difference from $f(g_0^{-1}x)$ is less than $\varepsilon$; a finite cover of $G$ permits one common [neighbourhood](../../../../../neighbourhood-mathematics.md) of $g_0$. Hence $\|l_gf-l_{g_0}f\|_\infty\to0$. The estimate

$$
\|l_gf-l_{g_0}f_0\|_\infty\leq\|f-f_0\|_\infty+\|l_gf_0-l_{g_0}f_0\|_\infty
$$

then proves the joint continuity of the action on $G\times C(G)$.

For a left action on the [continuous dual space](../../../../../continuous-dual-space-split.md), use the contragredient convention

$$
T_g\phi=\phi\circ l_{g^{-1}}.
$$

It satisfies $T_gT_h=T_{gh}$ and preserves the dual [unit ball](../../../../../unit-ball.md) $B'$. If the printed prime denotes the literal transpose $l_g^*\phi=\phi\circ l_g$, these maps instead satisfy $l_g^*l_h^*=l_{hg}^*$ and form a right action; replacing $g$ by $g^{-1}$ gives the left action above. Their invariant functionals are the same.

For $g_i\to g$ and $\phi_i\to\phi$ in the [weak-star topology](../../../../../weak-star-topology.md) on $B'$, every $f\in C(G)$ satisfies

$$
|(T_{g_i}\phi_i)(f)-(T_g\phi)(f)|\leq\|l_{g_i^{-1}}f-l_{g^{-1}}f\|_\infty+|(\phi_i-\phi)(l_{g^{-1}}f)|\longrightarrow0.
$$

The first term uses strong continuity of translation and $\|\phi_i\|\leq1$; the second uses weak-star convergence at one fixed function. This proves the requested joint [weak-star topology](../../../../../weak-star-topology.md) continuity.

To obtain [Haar measure](../../../../../haar-measure.md), consider the set $K$ of [positive linear functionals](../../../../../positive-linear-functional.md) $\phi$ on $C(G)$ with $\phi(1)=1$. Such functionals have [norm](../../../../../norm.md) one: for complex $f$, choose a phase making $\phi(f)$ real and nonnegative and use $\operatorname{Re}(e^{it}f)\leq\|f\|_\infty$; this gives $|\phi(f)|\leq\|f\|_\infty$, with equality on the constant-one function. Thus $K\subseteq B'$. Evaluation at the identity belongs to $K$, and positivity and normalization are weak-star closed conditions. The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) makes $K$ a nonempty compact convex set. Each $T_g$ is a continuous affine self-map of it.

Here is the fixed-point step, including why no [commutativity](../../../../../commutativity.md) assumption on $G$ is needed. For any finite list $g_1,\ldots,g_n$, the [Schauder-Tychonoff fixed-point theorem](../../../../../schauder-tychonoff-fixed-point-theorem.md) gives a fixed point $\phi\in K$ of $n^{-1}\sum_jT_{g_j}$. Let $H$ be the closed subgroup they generate and, for real $f\in C(G)$, set $h(x)=\phi(l_xf)$ on $H$. It is continuous and satisfies

$$
h(x)=\frac1n\sum_{j=1}^nh(g_j^{-1}x).
$$

At a maximum point $x_0$, every summand must have the same maximum value. Iteration gives that value at all inverse-generator words times $x_0$. The closure of their positive-word monoid is a [closed subsemigroup of a compact group](../../../../../closed-subsemigroup-of-a-compact-group.md), hence is the entire generated subgroup $H$. Density and continuity make $h$ constant on $H$. Therefore $\phi$ is fixed by each of $T_{g_1},\ldots,T_{g_n}$, first on real functions and then on complex functions by linearity. The closed fixed-point sets consequently have the [finite intersection property](../../../../../finite-intersection-property.md) in $K$, so compactness gives a common fixed functional for every $g\in G$.

The [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) converts this positive functional into a regular Borel [probability measure](../../../../../probability-measure.md) $\mu_l$ with $\phi(f)=\int f\,d\mu_l$. Its invariance gives left translation invariance of the [measure](../../../../../measure.md). It has full support: if a nonempty open set had [measure](../../../../../measure.md) zero, a finite collection of its left translates would cover the compact group and force $\mu_l(G)=0$, contradicting normalization. Thus it is a normalized left [Haar measure](../../../../../haar-measure.md). The right translation action gives a normalized right [Haar measure](../../../../../haar-measure.md) $\mu_r$ by the same argument.

For uniqueness and equality, take any $f\in C(G)$ and apply the [Fubini theorem](../../../../../fubini-s-theorem.md) to

$$
I=\int_G\int_G f(yx)\,d\mu_l(x)\,d\mu_r(y).
$$

For fixed $y$, left invariance of $\mu_l$ makes the inner integral $\int f\,d\mu_l$. Reversing the order, for fixed $x$, right invariance of $\mu_r$ makes the inner integral $\int f\,d\mu_r$. Since both total masses are one,

$$
\int f\,d\mu_l=I=\int f\,d\mu_r.
$$

Uniqueness in the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) gives $\boxed{\mu_l=\mu_r}$. Comparing any normalized left [Haar measure](../../../../../haar-measure.md) to this fixed right [Haar measure](../../../../../haar-measure.md) proves uniqueness as well. **The conclusion is uniqueness of normalized [Haar measure](../../../../../haar-measure.md).** Without normalization, the printed uniqueness claim is false: even on the one-point group, $\delta_e$ and $2\delta_e$ are distinct Haar [measures](../../../../../measure.md). In general the result is uniqueness up to a positive scalar, and left and right probability normalizations coincide.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
