<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $X$ be the vertex set of a [regular polygon](../../../../../regular-polygon.md) and let the cyclic rotation group $A$ act transitively on it. The finite invariant-colouring lemma says that for every number of colours there are positive weights $w_1,ldots,w_N$ with $\sum_iw_i^2=1$ such that every colouring of the weighted Cartesian power

$$
X_w^N=\{(w_1x_1,\ldots,w_Nx_N):x_i\in X\}
$$

contains a monochromatic set

$$
\{(w_1a x_1,\ldots,w_Na x_N):a\in A\}.
$$

For completeness, prove the lemma along a cyclic composition series for $A$. For a prime cyclic quotient, refine each colour to the finite vector of colours obtained by applying the quotient elements in every active coordinate. The [Hales-Jewett theorem](../../../../../hales-jewett-theorem.md) supplies a variable block on which this vector is constant. Assign that block squared weights summing to the squared weight of the coordinate it replaces. This makes the quotient orbit monochromatic without changing any orbit distance. Iterating through the cyclic factors proves the lemma for the finite cyclic group $A$.

Because rotations commute, for $a,b\in A$ each coordinate satisfies

$$
\|a x_i-bx_i\|=\|av-bv\|
$$

for a fixed vertex $v$. Hence the squared distance between the two corresponding product points is

$$
\sum_iw_i^2\|a x_i-bx_i\|^2
=\|av-bv\|^2.
$$

The monochromatic orbit is therefore isometric to $X$. This proves that every regular polygon is a [Euclidean Ramsey set](../../../../../regular-polygon-is-a-euclidean-ramsey-set.md).

Now consider the edge-colouring definition. If all pairwise distances in $X$ are equal, then $X$ is a regular simplex. Take a sufficiently large regular simplex $S$ of the same side length. The ordinary finite [Ramsey theorem](../../../../../ramsey-theorem.md) gives a monochromatic $|X|$-vertex complete subgraph, and every such vertex set is isometric to $X$. Thus $X$ is an [edge Ramsey set](../../../../../edge-ramsey-set.md).

Conversely, if $X$ has two distances, let $a$ and $b$ be its least and greatest distances. Colour every Euclidean edge by whether its length equals $a$. Every isometric copy of $X$ contains both an edge of length $a$ and one of length $b$, so no copy is monochromatic. Hence the edge Ramsey sets are exactly the equidistant finite sets.

Allowing similar copies does not change the answer. If $r=b/a>1$, colour an edge of length $d$ by the parity of

$$
\left\lfloor\log_r d\right\rfloor.
$$

In every similar copy, the images of a shortest and a longest edge have lengths $ta$ and $tb=rta$, whose displayed integers differ by one. They receive opposite colours. Thus no non-equidistant $X$ is edge Ramsey even up to similarity, while the regular-simplex argument already supplies an isometric copy.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
