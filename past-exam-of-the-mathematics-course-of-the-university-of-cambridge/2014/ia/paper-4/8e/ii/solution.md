<h1 id="8e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the ambient [set](../../../../../../set-split.md) of all $n^n$ [functions](../../../../../../function-split.md) from $\mathbb Z/n\mathbb Z$ to itself, let $A_j$ be the forbidden event $f(j)-f(j-1)\equiv j\pmod n$. Apply the avoidance form of the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) from part (i).

For a proper [subset](../../../../../../subset.md) $J$ of the $n$ [cyclic difference constraints](../../../../../../cyclic-difference-constraints.md), with $|J|=k<n$, the selected edges form disjoint paths around the cycle, including isolated vertices. There are $n-k$ components. On each component, choosing one value of $f$ arbitrarily determines all the other values by the prescribed differences. No consistency condition occurs because the cycle has been broken. Therefore

$$
\left|\bigcap_{j\in J}A_j\right|=n^{n-k}\qquad(k<n).
$$

This also works for $n=2$, whose two directed constraints use the same pair of vertices: any single constraint leaves one freely chosen value.

If all $n$ constraints hold, summing them around the cycle gives the necessary condition

$$
0\equiv\sum_{j=0}^{n-1}j=\frac{n(n-1)}2\pmod n.
$$

It holds when $n$ is odd and fails when $n$ is even, the latter sum being congruent to $n/2$. When it holds, choose $f(0)$ in $n$ ways and determine every other value; the final constraint is then consistent. Thus the full intersection has size $F=n$ for odd $n$ and $F=0$ for even $n$.

There are $\binom nk$ [subsets](../../../../../../subset.md) of size $k$. By the [binomial theorem](../../../../../../binomial-theorem.md),

$$
|X|=\sum_{k=0}^{n-1}(-1)^k\binom nk n^{n-k}+(-1)^nF
=(n-1)^n+(-1)^n(F-1).
$$

Hence **the number of admissible [functions](../../../../../../function-split.md) is**

$$
\boxed{|X|=\begin{cases}(n-1)^n+1-n,&n\text{ odd},\\(n-1)^n-1,&n\text{ even}.\end{cases}}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
