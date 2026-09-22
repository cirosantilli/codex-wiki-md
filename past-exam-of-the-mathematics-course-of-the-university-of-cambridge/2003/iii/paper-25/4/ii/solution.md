<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The graph form of [Plünnecke inequality](../../../../../../plunnecke-inequality.md) states

$$
\boxed{D_k(G)^{1/k}\ge D_n(G)^{1/n}\quad(1\le k\le n).}
$$

Equivalently these roots are nonincreasing along the layers. If $D_n=0$ the conclusion is immediate. Otherwise put $C=D_n^{1/n}$ and use the [weighted cut lemma for commutative graphs](../../../../../../weighted-cut-lemma-for-commutative-graphs.md) proved in part (i). For a minimum endpoint cut $S_0\cup S_n$,

$$
w(S_0\cup S_n)=|S_0|+D_n^{-1}|S_n|
\ge |S_0|+|V_0\setminus S_0|=|V_0|.
$$

The bottom layer is a cut of this weight. Comparing with $(V_0\setminus Z)\cup\operatorname{Im}^{(k)}Z$ gives $|\operatorname{Im}^{(k)}Z|\ge C^k|Z|$, as required. In an addition graph, $D_1\le K$ when $|A+B|\le K|A|$, so $D_m\le K^m$: some nonempty bottom subset has growth at most $K^m$ at height $m$.

The useful simultaneous [sumset](../../../../../../sumset.md) form says that a nonempty $X\subseteq A$ can be chosen with $|X+mB|\le K^m|X|$ for every $m$. To verify the common-subset assertion directly, choose $X$ minimizing $K'=|X+B|/|X|$ among subsets of $A$. For a finite set $T=\{t_1,\ldots,t_s\}$, let $X_i$ consist of those $x\in X$ for which $x+t_i$ is a new point of $X+T$. The translated $X_i$ partition $X+T$. Points contributed by $(X\setminus X_i)+B+t_i$ are already present in earlier translates of $X+B$, so the new contribution at stage $i$ has size at most

$$
|X+B|-|(X\setminus X_i)+B|
\le K'|X|-K'|X\setminus X_i|=K'|X_i|.
$$

The inequality also holds when the complementary set is empty. Summing gives $|X+B+T|\le K'|X+T|$. Taking $T=(m-1)B$ and iterating proves $|X+mB|\le(K')^m|X|\le K^m|X|$. This is the [Petridis minimal-growth lemma](../../../../../../petridis-minimal-growth-lemma.md) calculation and supplies a single subset for all needed heights.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
