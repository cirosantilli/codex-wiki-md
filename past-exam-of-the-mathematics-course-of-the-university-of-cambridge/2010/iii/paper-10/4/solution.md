<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [set family](../../../../../set-family.md) [shatters a set](../../../../../set-shattering.md) $Z$ when its traces on $Z$ include all of $\mathcal P(Z)$. The [Sauer-Shelah lemma](../../../../../sauer-shelah-lemma.md) says that a [set family](../../../../../set-family.md) $\mathcal F\subseteq\mathcal P([n])$ which shatters no $k$-set satisfies

$$
\boxed{|\mathcal F|\leq\sum_{i=0}^{k-1}\binom ni.}
$$

Equivalently, if $|\mathcal F|$ exceeds this sum, it shatters a $k$-set. [Binomial coefficients](../../../../../binomial-coefficient.md) with index greater than $n$ are zero; if $k>n$ the inequality reduces to the whole-power-set bound. The [VC dimension](../../../../../vc-dimension.md) formulation puts $k=d+1$.

We give the full inductive proof. Split $\mathcal F$ according to the last coordinate, deleting that coordinate from the present section, and write these two [set families](../../../../../set-family.md) on $[n-1]$ as $\mathcal F_0,\mathcal F_1$. Put

$$
\mathcal C=\mathcal F_0\cup\mathcal F_1,\qquad
\mathcal D=\mathcal F_0\cap\mathcal F_1.
$$

The [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) gives $|\mathcal F|=|\mathcal C|+|\mathcal D|$. If $\mathcal C$ shattered a $k$-set, then $\mathcal F$ would shatter it too. If $\mathcal D$ shattered a $(k-1)$-set $Z$, both versions of each required trace, with and without the last coordinate, would occur in $\mathcal F$, which would shatter $Z\cup\{n\}$. Thus the two [mathematical induction](../../../../../mathematical-induction.md) bounds apply:

$$
|\mathcal F|\leq\sum_{i=0}^{k-1}\binom{n-1}{i}
+\sum_{i=0}^{k-2}\binom{n-1}{i}
=\sum_{i=0}^{k-1}\binom ni,
$$

using [Pascal's identity](../../../../../pascal-s-rule.md). For $n=0$ the [set family](../../../../../set-family.md) has at most one member. For $k=1$, the intersection section must be empty, since any nonempty [set family](../../../../../set-family.md) shatters the empty [set](../../../../../set-split.md). These supply the [mathematical induction](../../../../../mathematical-induction.md) bases; the forbidden-empty-set case has an empty [set family](../../../../../set-family.md) and an empty sum. Sharpness is attained by all [subsets](../../../../../subset.md) of size at most $k-1$, which cannot shatter a $k$-set.

Now fix $k\geq1$ in the infinite-ground-set problem. Choose, using the hypothesis with $2k$, a [set](../../../../../set-split.md) $Y$ of size $2k$ with at least $2^{2k-1}$ distinct traces. If its trace [set family](../../../../../set-family.md) shattered no $k$-set, the [Sauer-Shelah lemma](../../../../../sauer-shelah-lemma.md) would give

$$
|\mathcal A_{|Y}|\leq\sum_{i=0}^{k-1}\binom{2k}{i}
=\frac{2^{2k}-\binom{2k}{k}}2
<2^{2k-1},
$$

a contradiction. Therefore some $Z\subseteq Y$ of size $k$ is shattered by the trace [set family](../../../../../set-family.md), and hence by $\mathcal A$ itself. Thus **every finite shattering size occurs**. The use of $2k$ makes the contradiction strict, even though the hypothesis only gives a half-power-set lower bound.

An infinite realization does not follow. For a concrete [unbounded finite shattering without an infinite universal trace](../../../../../unbounded-finite-shattering-without-an-infinite-universal-trace.md) construction, partition $X=\mathbb N$ into disjoint finite blocks

$$
B_j=\left\{\frac{j(j-1)}2+1,\ldots,\frac{j(j+1)}2\right\},\qquad |B_j|=j,
$$

and take

$$
\boxed{\mathcal A=\bigcup_{j\geq1}\mathcal P(B_j).}
$$

Every member is finite. Given $k$, choose $Y=B_k$; its trace [set family](../../../../../set-family.md) is the full [power set](../../../../../power-set.md), so it has $2^k\geq2^{k-1}$ members and is shattered. However, an infinite $Z$ cannot be contained in one finite block. Choose $x,y\in Z$ from different blocks. No member of $\mathcal A$ contains both, so $\{x,y\}$ is not a trace on $Z$. Consequently **there need not be an infinite $Z$ whose traces contain every finite [subset](../../../../../subset.md) of $Z$**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
