<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

For the [cofinite topology](../../../../../cofinite-topology.md) $\tau_1$, the empty set and $\mathbb N$ are included. A nonempty union of cofinite sets is cofinite because its complement is contained in the finite complement of any one member. A finite intersection is cofinite because its complement is a finite union of finite sets; intersections involving the empty set are empty. This proves all [topology](../../../../../topology-split.md) axioms.

For the [tail topology on the natural numbers](../../../../../tail-topology-on-the-natural-numbers.md) $\tau_2$, $\mathbb N=I_1$. Any nonempty collection of tails has a smallest starting index, so its union is that tail; a finite intersection of tails is the tail with largest starting index. Empty sets and empty-family conventions supply the remaining cases. Thus $\tau_2$ is also a [topology](../../../../../topology-split.md).

We classify [continuous maps between cofinite and tail topologies](../../../../../continuous-maps-between-cofinite-and-tail-topologies.md). [Continuity](../../../../../continuous-function.md) is equivalent to

$$
E_k=\{n:f(n)\ge k\}\text{ being empty or cofinite for every }k.
$$

If $f$ has unbounded image, each $E_k$ is nonempty, hence cofinite. For every threshold $k$, eventually $f(n)\ge k$, which is exactly $f(n)\to\infty$. If the image is bounded, it is a nonempty finite subset of $\mathbb N$ and has a maximum $N$. Then $E_N$ is nonempty and cofinite, but $f(n)\le N$ always, so $f(n)=N$ except at finitely many indices. These exhaust the two possibilities and prove necessity. Their sufficiency is checked separately below.

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
