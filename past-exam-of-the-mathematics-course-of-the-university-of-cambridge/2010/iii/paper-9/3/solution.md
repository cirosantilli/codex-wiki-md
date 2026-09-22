<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Call $A\subseteq\mathbb N$ an [IP set](../../../../../ip-set.md) when it contains an infinite [finite-sums set](../../../../../finite-sums-set.md) $\operatorname{FS}(x_1,x_2,\ldots)$ with all $x_i>0$. We first need the relative consequence of the [Hindman theorem](../../../../../hindman-theorem.md): **a finite union can be an [IP set](../../../../../ip-set.md) only if one of its constituents is an [IP set](../../../../../ip-set.md)**. This does not follow by simply applying the theorem to a coloring of all integers, because its [monochromatic](../../../../../monochromatic-set.md) [finite-sums set](../../../../../finite-sums-set.md) might lie outside the given set.

Here is a reduction that proves the [partition regularity of IP sets](../../../../../partition-regularity-of-ip-sets.md). Suppose $\operatorname{FS}(x_i)\subseteq A$ and $A$ is finitely colored. Index the generators by $i\geq0$. For $n>0$, let $S(n)$ be the set of positions of the nonzero digits in its [binary expansion](../../../../../binary-expansion.md), and color $n$ by the color of $\sum_{i\in S(n)}x_i$. By the [Hindman theorem](../../../../../hindman-theorem.md), there are $w_1,w_2,\ldots>0$ with $\operatorname{FS}(w_i)$ [monochromatic](../../../../../monochromatic-set.md) in this new [finite coloring](../../../../../finite-coloring.md).

We can take disjoint, successively later finite blocks of the $w_i$ whose sums $v_1,v_2,\ldots$ have separated [binary expansion](../../../../../binary-expansion.md) supports. Start with $v_1=w_1$. Having chosen finitely many blocks, take $K$ larger than every binary position used in their sums. On a fresh tail of the $w_i$, consider $2^K+1$ partial sums, including the zero partial sum. Two have the same [residue class](../../../../../residue-class.md) modulo $2^K$, by the [pigeonhole principle](../../../../../pigeonhole-principle.md). Their positive difference is a consecutive block sum $v_{j+1}$ divisible by $2^K$. Discard all indices up to that block's end and repeat. Thus every bit of $v_{j+1}$ is above every bit in the preceding block sums.

There are no carries in a sum of distinct $v_j$, so

$$
S\left(\sum_{j\in J}v_j\right)=\bigsqcup_{j\in J}S(v_j)\qquad(\varnothing\ne J\text{ finite}).
$$

Also $\operatorname{FS}(v_j)\subseteq\operatorname{FS}(w_i)$, since the underlying blocks are disjoint. Consequently

$$
y_j:=\sum_{i\in S(v_j)}x_i
$$

satisfies $\operatorname{FS}(y_j)\subseteq\operatorname{FS}(x_i)\subseteq A$, with all these sums the same original color. This proves the relative assertion. In particular, if $A_1\cup\cdots\cup A_r$ contains an infinite [finite-sums set](../../../../../finite-sums-set.md), color its points by the first constituent containing them and apply this argument; one $A_j$ is an [IP set](../../../../../ip-set.md).

Let $\mathcal I$ be the family of sets that are not [IP sets](../../../../../ip-set.md). It is closed under subsets and, by the preceding argument, under finite unions. It contains every [finite set](../../../../../finite-set.md), since positive successive partial sums of an infinite sequence are unbounded. It does not contain $\mathbb N$. Therefore

$$
\mathcal F=\{A\subseteq\mathbb N:A^c\in\mathcal I\}
$$

is a proper [filter on a set](../../../../../filter-set-theory.md): it contains $\mathbb N$, excludes the empty set, is upward closed, and is closed under finite intersections. Its members are exactly the [IP-star sets](../../../../../ip-star-set.md), the sets meeting every [IP set](../../../../../ip-set.md). Indeed, failure to meet an [IP set](../../../../../ip-set.md) is equivalent to having an IP complement. This identifies the sets that must belong to the required [ultrafilter](../../../../../ultrafilter.md).

Apply the [ultrafilter lemma](../../../../../ultrafilter-lemma.md) to extend the [IP-star filter](../../../../../ip-star-filter.md) $\mathcal F$ to an [ultrafilter](../../../../../ultrafilter.md) $\mathcal U$. For completeness, [Zorn lemma](../../../../../zorn-s-lemma.md) applies to its proper filter extensions ordered by inclusion, because the union of a chain is still a proper [filter on a set](../../../../../filter-set-theory.md). A maximal extension decides every set $A$: if $A$ cannot be adjoined while keeping the filter proper, some filter member is disjoint from $A$, forcing $A^c$ into the filter. This is the defining [ultrafilter](../../../../../ultrafilter.md) property.

If $A\in\mathcal U$ were not an [IP set](../../../../../ip-set.md), then $A^c\in\mathcal F\subseteq\mathcal U$, contradicting properness. Hence **every member of $\mathcal U$ contains an infinite [finite-sums set](../../../../../finite-sums-set.md)**. Conversely, any [ultrafilter with finite-sums members](../../../../../ultrafilter-with-finite-sums-members.md) must contain every [IP-star set](../../../../../ip-star-set.md), since it cannot contain such a set's non-IP complement. Thus this construction captures precisely the forced filter, without making an unnecessary claim about idempotence.

To prove nonuniqueness, put

$$
E=\bigcup_{j\geq0}\bigl([2^{2j},2^{2j+1})\cap\mathbb N\bigr).
$$

For a nonempty finite set of exponents with largest exponent $J$, the associated sum of distinct powers of four satisfies

$$
4^J\leq\sum_{j\in F}4^j\leq\frac{4^{J+1}-1}{3}<2\cdot4^J.
$$

Thus $\operatorname{FS}(4^j:j\geq0)\subseteq E$. Doubling the inequality gives

$$
2\cdot4^J\leq\sum_{j\in F}2\cdot4^j<4\cdot4^J,
$$

so $\operatorname{FS}(2\cdot4^j:j\geq0)\subseteq E^c$. These [alternating dyadic intervals contain disjoint IP sets](../../../../../alternating-dyadic-intervals-contain-disjoint-ip-sets.md).

Every member of $\mathcal F$ meets $E$ and also $E^c$, because it meets every [IP set](../../../../../ip-set.md). A finite intersection of members of $\mathcal F$ is again a member, so both $\mathcal F\cup\{E\}$ and $\mathcal F\cup\{E^c\}$ have the [finite intersection property](../../../../../finite-intersection-property.md). Extend the proper filters they generate to [ultrafilters](../../../../../ultrafilter.md) $\mathcal U_0$ and $\mathcal U_1$. Each extends $\mathcal F$, so the previous argument makes each an [ultrafilter with finite-sums members](../../../../../ultrafilter-with-finite-sums-members.md). But $E\in\mathcal U_0$ and $E^c\in\mathcal U_1$, so

$$
\boxed{\mathcal U_0\ne\mathcal U_1.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
