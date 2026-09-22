<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If the [random k-out graph](../../../../../../random-k-out-graph.md) with $k=2$ is disconnected, one of its [connected components of a graph](../../../../../../component-graph-theory.md) has size $3\le s\le n/2$. The lower bound follows because every [vertex](../../../../../../vertex-graph-theory.md) chooses two distinct neighbours inside its component. For a specified $s$-set $S$, absence of crossing [edges](../../../../../../edge-of-a-graph.md) requires every choice at a [vertex](../../../../../../vertex-graph-theory.md) in $S$ to stay in $S$, and every choice outside to stay outside. Independence of choices at different [vertices](../../../../../../vertex-graph-theory.md) gives exactly

$$
\Pr(S\text{ has no crossing edge})=\left[\frac{\binom{s-1}2}{\binom{n-1}2}\right]^s\left[\frac{\binom{n-s-1}2}{\binom{n-1}2}\right]^{n-s}.
$$

For $3\le s\le n/2$, the two ratios are at most $(s/n)^2$ and $(1-s/n)^2$. Indeed each of the factors $(s-j)/(n-j)$, $j=1,2$, is at most $s/n$, and the complementary statement is identical. Put $t=s/n$. The [binomial coefficient](../../../../../../binomial-coefficient.md) bound $\binom ns\le t^{-s}(1-t)^{-(n-s)}$ follows by bounding the [probability](../../../../../../probability.md) of $s$ successes in $\operatorname{Bin}(n,t)$ by one. Thus the [union bound](../../../../../../boole-s-inequality.md) gives

$$
\Pr(G_{2\text{-out}}\text{ disconnected})\le\sum_{s=3}^{\lfloor n/2\rfloor}t^s(1-t)^{n-s}\le\sum_{s=3}^{\lfloor n/2\rfloor}(s/n)^s.
$$

For $s\le\sqrt n$, the last summands are at most $n^{-s/2}$, whose sum from three tends to zero. For $s>\sqrt n$, they are at most $2^{-s}$, again summing to zero. Therefore

$$
\boxed{\Pr(G_{2\text{-out}}\text{ connected})=1-o(1).}
$$

The proof bounds all possible small components rather than assuming the dependent undirected [edges](../../../../../../edge-of-a-graph.md) behave like a [binomial random graph](../../../../../../binomial-random-graph.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
