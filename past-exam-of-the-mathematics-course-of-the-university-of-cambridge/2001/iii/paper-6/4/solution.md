<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [weak topology](../../../../../weak-topology-split.md) $\sigma(E,E^*)$ is the coarsest topology making every [continuous linear functional](../../../../../continuous-linear-functional.md) in $E^*$ continuous. A basic neighborhood of $x$ imposes finitely many inequalities $|f_j(z-x)|<\varepsilon$, and a [sequence](../../../../../sequence.md) converges weakly precisely when each $f(x_n)$ converges to $f(x)$. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) makes the dual separate points, so the [weak topology](../../../../../weak-topology-split.md) is Hausdorff.

Here is a proof of the requested weak subsequence property, the compact-to-sequential direction of the [Eberlein-Šmulian theorem](../../../../../eberlein-smulian-theorem.md). Let $Y$ be the closed linear span of the countable set $\{x_n:n\ge1\}$. It is a [separable Banach space](../../../../../separable-banach-space.md). The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) separates points outside a closed [vector subspace](../../../../../vector-subspace.md) from that subspace, so $Y$ is weakly closed in $E$. Therefore $C=K\cap Y$ is weakly compact.

Choose a countable dense set $(u_j)$ in the unit sphere of $Y$, and choose [norming functionals](../../../../../norming-functional.md) $f_j\in Y^*$ with $\|f_j\|=1$ and $f_j(u_j)=1$. They separate points: for $y\ne0$, a sufficiently close $u_j$ to $y/\|y\|$ gives $|f_j(y)|>0$. This is a [countable norming family](../../../../../countable-norming-family.md). Extend the functionals to $E$ by the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). The evaluation map

$$
C\longrightarrow\mathbb F^{\mathbb N},\qquad y\longmapsto(f_j(y))_{j\ge1}
$$

is weakly continuous and injective. Its domain is compact and its target Hausdorff, so it is a [homeomorphism](../../../../../homeomorphism.md) onto its image: images of closed subsets are compact, hence closed. A countable product of real or complex lines is metrizable, for example by $\sum_j2^{-j}\min(1,|a_j-b_j|)$. Thus $C$ has a compact metrizable weak topology. Compact [metric spaces](../../../../../metric-space.md) are sequentially compact, giving **a subsequence with $\boxed{x_{n_j}\rightharpoonup x\in C\subseteq K}$**. If $Y=\{0\}$ the result is immediate. We did not assert that a separable [Banach space](../../../../../banach-space-split.md) has a separable dual or that its weak topology is generally metrizable.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
