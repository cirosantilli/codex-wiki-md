<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let

$$
d=\inf_{x\in K}\lVert x\rVert>0,
\qquad
M=\sup_{x\in K}\lVert x\rVert<\infty.
$$

Choose positive $\varepsilon_n$ with $\prod_n(1+\varepsilon_n)<\infty$. We construct $x_n\in K$ inductively. Once $E_n=\operatorname{span}\{x_1,\ldots,x_n\}$ has been chosen, compactness of its unit sphere gives finitely many members of $X^*$ that almost norm every vector of $E_n$. Because $0\in\overline K^w$, the next $x_{n+1}$ may be chosen so that all those functionals are as small on it as required. Choosing the error relative to $d$ gives

$$
\left\lVert\sum_{j=1}^na_jx_j\right\rVert
\leq(1+\varepsilon_n)
\left\lVert\sum_{j=1}^{n+1}a_jx_j\right\rVert
$$

for all scalars $a_1,\ldots,a_{n+1}$. Indeed, if the last coefficient could threaten this estimate, $\lVert x_{n+1}\rVert\geq d$ first bounds that coefficient by a fixed multiple of the norm of the preceding sum; the selected norming functional then gives the displayed inequality. Iteration and the finite product bound satisfy the standard [basis criterion](../../../../../basis-selection-theorem.md), so $(x_n)$ is a [basic sequence](../../../../../basic-sequence.md) contained in $K$.

The same proof works for any Hausdorff locally convex vector topology $\tau$ weaker than the [weak topology](../../../../../weak-topology-split.md): on each finite-dimensional $E_n$, the $\tau$-continuous linear functionals still norm the space, and $0\in\overline K^\tau$ supplies the next point. A canonical strictly weaker example arises on $X^*$ when $X$ is not [reflexive](../../../../../reflexive-banach-space.md): the [weak-star topology](../../../../../weak-star-topology.md) $\sigma(X^*,X)$ is then strictly weaker than the weak topology $\sigma(X^*,X^{**})$.

We next prove the [Eberlein-Šmulian theorem](../../../../../eberlein-smulian-theorem.md). If the weak closure of a bounded set $K$ is weakly compact, take any sequence in $K$ and let $Y$ be its closed linear span. The relevant weak closure lies in the separable space $Y$. A countable weak-star dense subset of the dual unit ball separates points of this compact set, so its weak topology is metrizable. Compact metrizability gives a weakly convergent subsequence.

For the converse, suppose $K$ is not relatively weakly compact. In the canonical embedding into $X^{**}$, choose

$$
x^{**}\in\overline{J_XK}^{w^*}\setminus J_X(X).
$$

The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) gives $x^{***}\in X^{***}$ that vanishes on $J_X(X)$ but satisfies $x^{***}(x^{**})=1$. Alternating [Goldstine approximation](../../../../../goldstine-theorem.md) with the fact that $x^{**}$ lies in the weak-star closure of $J_XK$ constructs bounded $x_n^*\in X^*$ and $x_n\in K$ such that, up to errors tending to zero,

$$
x_i^*(x_j)=0\quad(j\leq i),
\qquad
x_i^*(x_j)=1\quad(i<j).
$$

If a subsequence $x_{n_j}$ converged weakly to $x$, then for each fixed $i$ the second relation would give $x_i^*(x)=1$. A weak-star cluster point $x^*$ of the bounded sequence $(x_i^*)$ satisfies $x^*(x_{n_j})=0$ by the first relation, and hence $x^*(x)=0$ by weak convergence; but passing to the same cluster point in $x_i^*(x)=1$ gives $x^*(x)=1$. This contradiction produces a sequence in $K$ with no weakly convergent subsequence. Relative weak compactness is therefore equivalent to the subsequence condition.

Finally suppose $K$ is weakly sequentially compact and $x\in\overline K^w$. If $x$ lies in the norm closure of $K$, a norm-convergent sequence suffices. Otherwise apply the first part to $K-x$ and obtain a basic sequence $(y_n)$. A subsequence converges weakly by hypothesis. Its weak limit lies in the closed span of the basic sequence, while every coordinate functional is eventually zero on that subsequence. The limit is consequently zero, so the corresponding sequence from $K$ converges weakly to $x$.

This also shows that a weakly sequentially compact $K$ is weakly closed: any point of its weak closure is the limit of a sequence in $K$, and a weakly convergent subsequence has its limit in $K$. The relative form of the [Eberlein-Šmulian theorem](../../../../../eberlein-smulian-theorem.md) then makes $K$ weakly compact. The reverse implication follows from the first direction of that theorem. Thus weak compactness and weak sequential compactness are equivalent.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
