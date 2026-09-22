<h1 id="1a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here [equivalent metrics](../../../../../../equivalence-of-metrics.md) means that the two [metrics](../../../../../../metric.md) induce the same [topology](../../../../../../topology-split.md), and [Lipschitz equivalent norms](../../../../../../equivalent-norms.md) means that there are constants $c,C>0$ such that $cp(x)\le q(x)\le Cp(x)$ for every $x$.

Suppose first that the inequalities hold. Since they also hold for $x-y$, the identity maps between the two [metric spaces](../../../../../../metric-space.md) are [Lipschitz continuous](../../../../../../lipschitz-continuity.md). In particular, each is continuous, so the [topologies](../../../../../../topology-split.md) agree.

Conversely, equality of the [topologies](../../../../../../topology-split.md) makes the identity from the $p$-[norm](../../../../../../norm.md) to the $q$-[norm](../../../../../../norm.md) continuous at zero. There is therefore $\delta>0$ such that $p(x)<\delta$ implies $q(x)<1$. For nonzero $x$, apply this to $\delta x/(2p(x))$ and use the absolute homogeneity of both [norms](../../../../../../norm.md):

$$
q(x)<\frac{2}{\delta}p(x).
$$

The reverse identity is also continuous, so there is $\varepsilon>0$ with $q(x)<\varepsilon\Rightarrow p(x)<1$. Rescaling again gives $p(x)<2q(x)/\varepsilon$. Thus

$$
\boxed{\frac{\varepsilon}{2}p(x)\le q(x)\le\frac{2}{\delta}p(x).}
$$

The inequalities also hold at zero. This is [topology determines norm equivalence](../../../../../../topology-determines-norm-equivalence.md); it works in arbitrary dimension because the rescaling argument needs neither a [basis](../../../../../../basis.md) nor compactness of a unit sphere.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1A](../../1a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
