<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $\kappa=|X|$, an infinite [cardinal number](../../../../../cardinal-number.md). The original PDF has the double exponent $2^{2^{|X|}}$; the single-exponent expression in the TeX aid is a transcription error.

We explicitly construct an [independent family of subsets](../../../../../independent-family-of-sets.md) with $2^\kappa$ members on a set of size $\kappa$. Let

$$
D=\{(s,H):s\in[\kappa]^{<\omega},\ H\subseteq\mathcal P(s)\}.
$$

For each finite $s$ there are finitely many possibilities for $H$. The collection of finite subsets of an infinite cardinal has size $\kappa$, so $|D|\le\kappa$; the points $(\{\xi\},\varnothing)$ give the reverse bound. Thus $|D|=\kappa$.

For every $B\subseteq\kappa$ define

$$
A_B=\{(s,H)\in D:B\cap s\in H\}.
$$

To verify independence, take distinct $B_1,\ldots,B_n$ and bits $\varepsilon_1,\ldots,\varepsilon_n$. For each pair $i<j$, choose a point of $B_i\mathbin{\triangle}B_j$ and let $s$ contain all these finitely many points. The traces $B_i\cap s$ are pairwise distinct. Set

$$
H=\{B_i\cap s:\varepsilon_i=1\}.
$$

Then $(s,H)\in A_{B_i}$ exactly for those $i$ with $\varepsilon_i=1$. Every finite Boolean pattern is therefore realized. The cases $n=0,1$ work by the same definition, allowing $s=\varnothing$. In particular the sets $A_B$ are all distinct, so the [finite-trace independent family construction](../../../../../fichtenholz-kantorovich-independent-family.md) gives exactly $2^\kappa$ independent members.

For each [function](../../../../../function-split.md) $\varepsilon:\mathcal P(\kappa)\to\{0,1\}$, prescribe $A_B$ when $\varepsilon(B)=1$ and $D\setminus A_B$ when $\varepsilon(B)=0$. Independence gives the [finite intersection property](../../../../../finite-intersection-property.md). Their finite intersections generate a proper [filter on a set](../../../../../filter-set-theory.md): its members are the subsets of $D$ containing one of those intersections.

To extend this to an [ultrafilter](../../../../../ultrafilter.md), order its proper filter extensions by inclusion. The union of a chain is again a proper filter, so [Zorn's lemma](../../../../../zorn-s-lemma.md) supplies a maximal one, $U_\varepsilon$. If neither a subset $Y$ nor its complement belonged to this filter, adjoining $Y$ would still generate a proper filter: otherwise some existing member would be disjoint from $Y$ and force its complement into the filter already. Maximality therefore gives the ultrafilter dichotomy. Using the ambient [axiom of choice](../../../../../axiom-of-choice.md), choose such an extension for every $\varepsilon$.

Distinct functions differ at some $B$. Their ultrafilters respectively contain $A_B$ and its complement, and cannot be equal. There are $2^{2^\kappa}$ such functions. Transporting the ultrafilters along a [bijection](../../../../../bijection.md) $D\to X$ proves the lower bound. The upper bound is immediate because every ultrafilter is a subset of $\mathcal P(X)$:

$$
2^{2^\kappa}\le|\operatorname{Ult}(X)|
\le|\mathcal P(\mathcal P(X))|=2^{2^\kappa}.
$$

Thus the [number of ultrafilters on an infinite set](../../../../../number-of-ultrafilters-on-an-infinite-set.md) is

$$
\boxed{|\operatorname{Ult}(X)|=2^{2^{|X|}}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
