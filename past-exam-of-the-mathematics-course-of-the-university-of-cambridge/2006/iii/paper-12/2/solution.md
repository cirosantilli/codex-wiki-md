<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Identify the [hypercube graph](../../../../../hypercube-graph.md) $Q_n$ with subsets of $[n]$, adjacent when they differ by one element. Write $N(\mathcal F)$ for a family's closed [vertex neighbourhood](../../../../../vertex-neighbourhood.md). The [simplicial order on the discrete cube](../../../../../simplicial-order-on-the-discrete-cube.md) orders first by size and then, within a rank, by [lexicographic order](../../../../../lexicographic-order.md): the least element of a [symmetric difference](../../../../../symmetric-difference.md) belongs to the earlier set. The [Harper theorem](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) says that if $I$ is the initial simplicial segment with $|I|=|\mathcal F|$, then

$$
\boxed{|N(\mathcal F)|\ge|N(I)|.}
$$

Equivalently this minimizes the [external vertex boundary](../../../../../external-vertex-boundary.md) at fixed [cardinality](../../../../../cardinality.md). This is the vertex-isoperimetric assertion, distinct from the edge version in Question 3.

Here is the deduction of [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md). For a family $\mathcal B\subseteq[n]^{(k)}$, adjoin every lower rank and set $\mathcal D=[n]^{(<k)}\cup\mathcal B$. For $k\ge1$,

$$
N(\mathcal D)=[n]^{(\le k)}\cup\nabla\mathcal B.
$$

The corresponding simplicial [initial segment](../../../../../initial-segment.md) is $[n]^{(<k)}\cup L$, where $L$ is the rank-$k$ lexicographic [initial segment](../../../../../initial-segment.md) of size $|\mathcal B|$. Canceling the common lower-rank count in Harper's inequality gives $|\nabla\mathcal B|\ge|\nabla L|$. The rank-zero case is immediate by considering its two possible families.

To turn upper shadows into lower shadows, let $\rho(i)=n+1-i$ and $T(B)=\rho([n]\setminus B)$. This bijection reverses inclusion and changes rank $k$ to $n-k$. If $B$ precedes $C$ in lex order, the largest element of $T(B)\triangle T(C)$ belongs to $T(C)$, so $T(B)$ precedes $T(C)$ in [colexicographic order](../../../../../colexicographic-order.md). Also $T(\nabla\mathcal B)=\partial(T\mathcal B)$. Hence applying the upper-shadow conclusion to the transformed family proves

$$
\boxed{|\partial\mathcal A|\ge|\partial C|,}
$$

where $C$ is the colex [initial segment](../../../../../initial-segment.md) of the same size and rank as $\mathcal A$. This is the Kruskal-Katona lower-shadow theorem. A colex segment's shadow is itself a colex segment: split its sets by their largest element, giving a full initial block of the preceding ground set followed by an initial block with the new largest element. The same description holds one rank lower. Iteration therefore shows that colex segments minimize shadows at every lower rank. This proves the [Harper theorem implies the Kruskal-Katona theorem](../../../../../harper-theorem-implies-the-kruskal-katona-theorem.md) deduction, including the necessary complement and coordinate reversal.

The [Erdős-Ko-Rado theorem](../../../../../erdos-ko-rado-theorem.md) states that for $1\le r\le n/2$, every [intersecting family](../../../../../intersecting-family.md) $\mathcal A\subseteq[n]^{(r)}$ satisfies

$$
\boxed{|\mathcal A|\le\binom{n-1}{r-1}.}
$$

The family of all $r$-sets containing a fixed point attains the bound. We use the standard convention of positive ranks here.

For the first proof, let $\mathcal B$ be the complements of members of $\mathcal A$, at rank $k=n-r\ge r$, and let $\mathcal S$ be its rank-$r$ [lower shadow](../../../../../lower-shadow.md). It is disjoint from $\mathcal A$, since $A\subseteq[n]\setminus A'$ would make two family members disjoint. Suppose $|\mathcal A|>\binom{n-1}{r-1}=\binom{n-1}k$. The colex rank-$k$ segment of that size contains every $k$-set on $[n-1]$ and at least one set containing $n$. Its rank-$r$ shadow therefore contains all $\binom{n-1}r$ old $r$-sets and at least one new $r$-set containing $n$. The iterated Kruskal-Katona bound gives

$$
|\mathcal S|>\binom{n-1}r.
$$

Then $|\mathcal A|+|\mathcal S|>\binom{n-1}{r-1}+\binom{n-1}r=\binom nr$, impossible for disjoint subfamilies of rank $r$. This proves the [Erdős-Ko-Rado theorem from shadows](../../../../../erdos-ko-rado-theorem-from-shadows.md).

For the second proof use the [Katona circle method](../../../../../katona-circle-method.md). In any [cyclic ordering](../../../../../cyclic-ordering.md) of the $n$ points, an intersecting collection of length-$r$ intervals has at most $r$ members. To prove this, rotate one selected interval to end at position $n$, so it occupies $n-r+1,\ldots,n$. Intervals ending at $r,\ldots,n-r$ miss it and cannot be selected. Among the remaining endpoints other than $n$, pair $j$ with $j+n-r$ for $1\le j\le r-1$. The two intervals in each pair are disjoint because $n\ge2r$, so at most one can be selected. Including the fixed interval gives at most $1+(r-1)=r$.

Now count pairs consisting of a family member and a [permutation](../../../../../permutation.md) in which it is a cyclic interval. A fixed $r$-set has $nr!(n-r)!$ such [permutations](../../../../../permutation.md): choose its final position, its internal order, and the order of the remaining points. Each of the $n!$ [permutations](../../../../../permutation.md) contributes at most $r$ family intervals by the proved [cyclic interval intersection bound](../../../../../cyclic-interval-intersection-bound.md). Thus

$$
|\mathcal A|nr!(n-r)!\le rn!,\qquad
|\mathcal A|\le\frac rn\binom nr=\binom{n-1}{r-1}.
$$

This is the required cyclic-ordering proof, with its interval lemma established explicitly.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
