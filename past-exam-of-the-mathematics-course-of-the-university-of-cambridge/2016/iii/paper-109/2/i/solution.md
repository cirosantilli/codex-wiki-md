<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Identify the [Boolean hypercube](../../../../../../boolean-hypercube.md) $Q_n$ with the subsets of $[n]$. For a family $\mathcal H$, write $N(\mathcal H)$ for its closed [vertex neighbourhood](../../../../../../vertex-neighbourhood.md), consisting of the family and all vertices at [Hamming distance](../../../../../../hamming-distance.md) one from it. Order subsets first by increasing size and, within a fixed size, use [lexicographic order](../../../../../../lexicographic-order.md): at the smallest coordinate on which they differ, the set containing that coordinate comes first. This is the [simplicial order on the discrete cube](../../../../../../simplicial-order-on-the-discrete-cube.md). **Harper's theorem** states that if $I$ is its initial segment of size $|\mathcal H|$, then

$$
\boxed{|N(\mathcal H)|\geq|N(I)|.}
$$

Thus simplicial initial segments minimize the [external vertex boundary](../../../../../../external-vertex-boundary.md) for each prescribed family size. The closed-neighbourhood and external-boundary formulations are equivalent because $|N(\mathcal H)\setminus\mathcal H|=|N(\mathcal H)|-|\mathcal H|$. No [edge boundary](../../../../../../edge-boundary-in-a-graph.md) is involved in this assertion.

We now give the deduction [Harper theorem implies the Kruskal-Katona theorem](../../../../../../harper-theorem-implies-the-kruskal-katona-theorem.md), keeping track of the two different orders. For a family $\mathcal F$ of $r$-sets with $r\geq1$, adjoin every smaller set:

$$
\mathcal H=\bigcup_{j<r}\binom{[n]}j\ \cup\ \mathcal F.
$$

Its closed [vertex neighbourhood](../../../../../../vertex-neighbourhood.md) is exactly

$$
N(\mathcal H)=\bigcup_{j\leq r}\binom{[n]}j\ \cup\ \nabla\mathcal F,
$$

where $\nabla\mathcal F$ is the [upper shadow](../../../../../../upper-shadow.md). Applying [Harper theorem](../../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) to $\mathcal H$ shows that, among $r$-uniform families of fixed size, the [lexicographic](../../../../../../lexicographic-order.md) [initial segment](../../../../../../initial-segment.md) minimizes the [upper shadow](../../../../../../upper-shadow.md): all the lower-level contributions to the two neighbourhood sizes are identical.

To convert this into a statement about the [lower shadow](../../../../../../lower-shadow.md) of a $k$-uniform family $\mathcal G$, take $r=n-k$ and map each member $S$ to $R([n]\setminus S)$, where $R(i)=n+1-i$ reverses the ground-set coordinates. Complementation changes [lower shadows](../../../../../../lower-shadow.md) to [upper shadows](../../../../../../upper-shadow.md), and the coordinate reversal preserves their sizes. Moreover, the resulting [lexicographic order](../../../../../../lexicographic-order.md) corresponds exactly to [colexicographic order](../../../../../../colexicographic-order.md) on the original $k$-sets: $S$ precedes $T$ in [colexicographic order](../../../../../../colexicographic-order.md) precisely when the largest element of $S\triangle T$ lies in $T$. After complementation and reversal, the smallest differing coordinate lies in the image of $S$, as required for the stated [lexicographic order](../../../../../../lexicographic-order.md). Hence **a [colexicographic](../../../../../../colexicographic-order.md) [initial segment](../../../../../../initial-segment.md) minimizes the [lower shadow](../../../../../../lower-shadow.md)**, which is the [Kruskal-Katona theorem](../../../../../../kruskal-katona-theorem.md). The cases $k=n$ and $k=0$ are immediate and need no adjoining construction.

For its usual numerical form, write the unique greedy [binomial representation](../../../../../../combinatorial-number-system.md)

$$
m=\binom{a_k}k+\binom{a_{k-1}}{k-1}+\cdots+\binom{a_t}t,\qquad a_k>a_{k-1}>\cdots>a_t\geq t\geq1.
$$

Then the [Kruskal-Katona theorem](../../../../../../kruskal-katona-theorem.md) says

$$
\boxed{|\partial\mathcal G|\geq\binom{a_k}{k-1}+\binom{a_{k-1}}{k-2}+\cdots+\binom{a_t}{t-1}\quad(|\mathcal G|=m).}
$$

Here is why the shadow of the [colexicographic](../../../../../../colexicographic-order.md) [initial segment](../../../../../../initial-segment.md) has exactly that size. Its first block consists of all $k$-sets in $[a_k]$. If any members remain, they have the form $\{a_k+1\}\cup T$, where $T$ runs through a [colexicographic](../../../../../../colexicographic-order.md) [initial segment](../../../../../../initial-segment.md) of $(k-1)$-sets. The [lower shadow](../../../../../../lower-shadow.md) consists of all $(k-1)$-sets in $[a_k]$, together with $\{a_k+1\}$ adjoined to the [lower shadow](../../../../../../lower-shadow.md) of that remainder. These two blocks are disjoint. Recursing gives precisely the displayed sum. For $m=0$, both the initial segment and its shadow are empty.

**The Erdős-Ko-Rado theorem** states that an [intersecting family](../../../../../../intersecting-family.md) $\mathcal A\subseteq\binom{[n]}r$, with $1\leq r\leq n/2$, satisfies

$$
\boxed{|\mathcal A|\leq\binom{n-1}{r-1}.}
$$

The bound is attained by all $r$-sets containing one fixed element. For the proof [Erdős-Ko-Rado theorem from shadows](../../../../../../erdos-ko-rado-theorem-from-shadows.md), take complements to obtain an $(n-r)$-uniform family $\mathcal B$ of the same size, and let $D$ be its rank-$r$ [lower shadow](../../../../../../lower-shadow.md). Every member of $D$ is disjoint from some member of $\mathcal A$, so $D\cap\mathcal A=\varnothing$. Iterating the [Kruskal-Katona theorem](../../../../../../kruskal-katona-theorem.md) bounds $|D|$ below by the rank-$r$ shadow of the [colexicographic](../../../../../../colexicographic-order.md) [initial segment](../../../../../../initial-segment.md) of size $|\mathcal B|$. This iteration is valid because [lower shadows](../../../../../../lower-shadow.md) of [colexicographic](../../../../../../colexicographic-order.md) [initial segments](../../../../../../initial-segment.md) are again [colexicographic](../../../../../../colexicographic-order.md) [initial segments](../../../../../../initial-segment.md), as the preceding block description shows.

If $|\mathcal A|>\binom{n-1}{r-1}=\binom{n-1}{n-r}$, that initial segment contains all $(n-r)$-sets in $[n-1]$ and at least one further set containing $n$. Since $r\leq n-r\leq n-1$, its rank-$r$ shadow contains every $r$-set in $[n-1]$ and at least one $r$-set containing $n$. Thus $|D|>\binom{n-1}r$, implying

$$
|D|+|\mathcal A|>\binom{n-1}r+\binom{n-1}{r-1}=\binom nr,
$$

contrary to their disjointness. This proves the bound. If $r>n/2$, all $r$-sets intersect and the trivial maximum is instead $\binom nr$.

For an [intersecting family in a product alphabet](../../../../../../intersecting-family-in-a-product-alphabet.md), label the alphabet by $\mathbb Z/k\mathbb Z$. Partition the words into the classes

$$
\{(x_1+t,\ldots,x_n+t):t\in\mathbb Z/k\mathbb Z\}.
$$

Each class has $k$ words, and any two distinct words in it disagree in every coordinate. An intersecting family therefore contains at most one word per class. There are $k^{n-1}$ classes, and fixing the first coordinate gives an intersecting family of that size. Consequently **the exact maximum is**

$$
\boxed{k^{n-1}\qquad(n\geq1,\ k\geq1).}
$$

For $k=1$ this just says that the single word may be included.

Finally, for a [weakly intersecting family in a product alphabet](../../../../../../weakly-intersecting-family-in-a-product-alphabet.md), associate to each word its support $S(x)=\{i:x_i>1\}$. The occurring supports form an [intersecting family](../../../../../../intersecting-family.md) of nonempty subsets, and the fibre over support $S$ has $(k-1)^{|S|}$ words. Put $w=k-1$. When $k\geq2$, $w\geq1$, and a support family can contain at most one of each complementary pair $S,[n]\setminus S$. For odd $n$, the larger support in each pair has size greater than $n/2$, so

$$
|\mathcal A|\leq\sum_{\{S,S^c\}}\max\{w^{|S|},w^{n-|S|}\}=\sum_{j>n/2}\binom nj(k-1)^j.
$$

All supports of size greater than $n/2$ are mutually intersecting, so taking every word over those supports achieves this bound. Thus **the required extremal family is the strict-majority support family**, with size

$$
\boxed{\sum_{j=(n+1)/2}^n\binom nj(k-1)^j.}
$$

This is the [weighted intersecting family bound on an odd Boolean lattice](../../../../../../weighted-intersecting-family-bound-on-an-odd-boolean-lattice.md). For $k>2$, strict inequality between the complementary fibre weights forces this extremal family to be unique. For $k=2$, it is a largest family but need not be the only one; for example, all supports containing one fixed coordinate also attain the same size. For $k=1$, no word has a nonempty support, so the maximum is zero, again agreeing with the formula.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
