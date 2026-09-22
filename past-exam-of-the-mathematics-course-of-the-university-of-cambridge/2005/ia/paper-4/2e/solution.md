<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

For nonnegative [integers](../../../../../integer.md) $n,m$, the [binomial coefficient](../../../../../binomial-coefficient.md) $\binom nm$ counts the $m$-element [subsets](../../../../../subset.md) of a fixed $n$-element set. It is zero when $m>n$, and $\binom n0=1$, including $n=0$. For $0\le m\le n$, taking the complement is a [bijection](../../../../../bijection.md) from $m$-element [subsets](../../../../../subset.md) to $(n-m)$-element [subsets](../../../../../subset.md); taking a complement twice gives the identity. Hence

$$
\boxed{\binom nm=\binom n{n-m}.}
$$

For $0\le l\le k\le n$, count ordered pairs $(L,K)$ of [subsets](../../../../../subset.md) of an $n$-element set with $L\subseteq K$, $|L|=l$ and $|K|=k$. Choosing $K$ first and then $L$ gives $\binom nk\binom kl$. Choosing $L$ first and then the $k-l$ additional elements of $K$ from its complement gives $\binom nl\binom{n-l}{k-l}$. These count the same pairs, proving the [nested-subset binomial identity](../../../../../nested-subset-binomial-identity.md):

$$
\boxed{\binom nk\binom kl=\binom nl\binom{n-l}{k-l}.}
$$

For the [Vandermonde identity](../../../../../vandermonde-s-identity.md), let disjoint sets $A,B$ have cardinalities $m,n$. A $k$-element [subset](../../../../../subset.md) of $A\cup B$ contains some number $i$ of elements of $A$. For a fixed $i$, there are $\binom mi\binom n{k-i}$ choices. The classes for different $i$ are disjoint and exhaust all $k$-element [subsets](../../../../../subset.md), so [double counting](../../../../../double-counting-proof-technique.md) gives

$$
\boxed{\sum_{i=0}^k\binom mi\binom n{k-i}=\binom{m+n}k.}
$$

The zero convention makes this valid for all nonnegative $m,n,k$, even if $k>m+n$. No factorial cancellation is needed for either counting proof.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
