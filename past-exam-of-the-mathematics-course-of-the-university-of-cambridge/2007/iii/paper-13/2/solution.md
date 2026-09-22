<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The claimed sufficient condition is false for the printed all-colours requirement.** This is a [polychromatic hypergraph colouring](../../../../../polychromatic-hypergraph-colouring.md) problem, which is stronger than merely avoiding monochromatic edges.

For a counterexample even with $k=3$, take $V=\{1,2,3,4\}$ and all four triples as edges. Every edge meets the other three, so $m=3$, and

$$
e(2m+2)=8e<27=3^k.
$$

Any assignment of three colours to four vertices repeats a colour on a pair. Any triple containing that pair has at most two colours. Thus this [uniform hypergraph](../../../../../uniform-hypergraph.md) satisfies the numerical hypothesis but has no required colouring. A single two-vertex edge would already provide a smaller counterexample if $k=2$ is allowed.

Here is the [correlation graph of events](../../../../../correlation-graph-of-events.md) argument that correctly applies to the printed colouring definition. Colour each vertex independently and uniformly with three colours, and let $B_E$ be the event that edge $E$ misses some colour. For $k\geq1$, the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) gives

$$
q:=\mathbb P(B_E)=3(2/3)^k-3(1/3)^k.
$$

Join two bad events when their edges intersect. This is a [dependency graph of events](../../../../../dependency-graph-of-events.md), hence also a [correlation graph of events](../../../../../correlation-graph-of-events.md), of maximum degree at most $m$: each $B_E$ depends only on colours on $E$, which are jointly independent of the colours on all disjoint edges. Precisely, the symmetric [Lovász local lemma](../../../../../lovasz-local-lemma.md) says that events of probability at most $q$ with such a graph have positive simultaneous avoidance [probability](../../../../../probability.md) whenever $eq(m+1)\leq1$. It follows from the asymmetric form $q\leq x(1-x)^m$, taking $x=1/(m+1)$ for $m\geq1$ and using $(m/(m+1))^m\geq e^{-1}$; the case $m=0$ is direct independence.

Thus a valid replacement sufficient condition is

$$
\boxed{e(m+1)\left[3(2/3)^k-3(1/3)^k\right]\leq1,}
$$

or the simpler, stronger condition $3e(m+1)\leq(3/2)^k$. Under either replacement, avoiding all $B_E$ gives exactly the requested [polychromatic hypergraph colouring](../../../../../polychromatic-hypergraph-colouring.md). For infinitely many vertices, finite subfamilies can be coloured and compactness of the product of three-point spaces extends this to all constraints; positive simultaneous avoidance probability is only asserted for finite families. The printed $3^k$ bound cannot be justified by substituting monochromatic-event probabilities for missing-colour probabilities.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
