<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Plünnecke graph](../../../../../../plunnecke-graph.md) is a finite directed layered graph $V_0,\ldots,V_n$, with edges only from $V_i$ to $V_{i+1}$, satisfying two commutation conditions. For each edge $u\to v$, the successors of $v$ can be matched injectively into the successors of $u$, so that the matched predecessor has an edge to the original successor. Dually, the predecessors of $u$ can be matched injectively into the predecessors of $v$, so that each original predecessor has an edge to its match. These are upward and downward commutation. For nonempty bottom subsets define the [graph magnification ratio](../../../../../../graph-magnification-ratio.md)

$$
D_k(G)=\min_{\varnothing\ne Z\subseteq V_0}
\frac{|\operatorname{Im}^{(k)}(Z)|}{|Z|}.
$$

Addition graphs have layer $A+iB$ and edges $x\to x+b$: exchanging the order of two additions gives exactly these matchings.

We prove a slightly stronger [weighted cut lemma for commutative graphs](../../../../../../weighted-cut-lemma-for-commutative-graphs.md), which also explains part (ii). Give vertices in $V_i$ weight $C^{-i}$, for any $C>0$. A separating set meets every bottom-to-top path. **There is a minimum-weight separating set contained in $V_0\cup V_n$.** We first establish its local three-layer step.

Consider a three-layer channel $U_0,U_1,U_2$, every vertex of which lies on a full path, and suppose the middle layer is a minimum-weight cut. Replacing a subset $Z\subseteq U_1$ by all its successors or all its predecessors still gives a cut. Minimality implies

$$
|\Gamma^+(Z)|\ge C|Z|,\qquad |\Gamma^-(Z)|\ge C^{-1}|Z|.
$$

Let $X_i\subseteq U_1$ be the vertices of incoming degree $i$. Partition $U_2$ into $T_i$ according to the largest incoming degree of one of their predecessors. Then

$$
\Gamma^+\left(\bigcup_{i\ge j}X_i\right)=\bigcup_{i\ge j}T_i,
\qquad \sum_{i\ge j}|T_i|\ge C\sum_{i\ge j}|X_i|.
$$

Downward commutation makes incoming degree nondecreasing along an edge. Thus every vertex of $T_i$ has at least $i$ predecessors, and summing the last inequalities over $j$ gives

$$
|E(U_1,U_2)|\ge\sum_i i|T_i|
\ge C\sum_i i|X_i|=C|E(U_0,U_1)|.
$$

Reverse all edges and interchange the endpoint layers. The graph still satisfies both commutation conditions, and the expansion factor becomes $C^{-1}$. The same argument now gives the opposite inequality $|E(U_0,U_1)|\ge C^{-1}|E(U_1,U_2)|$. Equality must therefore hold at every step. In particular the suffix inequality at $j=1$ is an equality, and the reversed argument gives

$$
|U_2|=C|U_1|,\qquad |U_0|=C^{-1}|U_1|.
$$

Consequently the bottom layer has exactly the middle layer's weight. This proves the local replacement lemma.

For a general minimum cut $S$, write $S_i=S\cap V_i$, and take its highest nonempty intermediate portion $S_j$, $0<j<n$. Form the three-layer channel whose bottom vertices are reachable from $V_0$ while avoiding the earlier cut portions, and whose top vertices can reach $V_n\setminus S_n$. Its middle layer is exactly $S_j$: any other middle vertex would produce an uncut full path, while every member of $S_j$ is essential in a positive-weight minimum cut and hence lies on such a path when that vertex alone is allowed. Channels inherit the commutation matchings: the replacement intermediate vertices still join the same prefix and suffix paths.

The middle layer is a minimum cut within this channel, since a cheaper local separator would replace $S_j$ and make the global cut cheaper. Apply the local lemma, with weights scaled by the common factor $C^{-(j-1)}$, to replace $S_j$ by the channel's bottom layer. This does not increase weight and removes the highest intermediate cut layer. Repetition leaves a minimum cut in the endpoint layers, proving the weighted cut lemma. Vertices lying on no full path can first be deleted; when $D_n>0$ all bottom vertices survive, and deleting such branches can only decrease intermediate images, so proving the lower bounds in the channel suffices.

Now take $C=1$ and assume $D_n\ge1$. If a minimum endpoint cut is $S_0\cup S_n$, then $\operatorname{Im}^{(n)}(V_0\setminus S_0)\subseteq S_n$, so

$$
|S_0|+|S_n|\ge|S_0|+|V_0\setminus S_0|=|V_0|.
$$

The bottom layer itself is a cut, so the minimum cut size is $|V_0|$. For every nonempty $Z\subseteq V_0$, the set $(V_0\setminus Z)\cup\operatorname{Im}^{(k)}Z$ is also a cut. Its size must be at least $|V_0|$, proving

$$
\boxed{|\operatorname{Im}^{(k)}Z|\ge|Z|,\qquad D_k(G)\ge1\quad(k\le n).}
$$

One may also apply the permitted [Menger theorem](../../../../../../menger-theorem.md) to obtain $|V_0|$ vertex-disjoint full paths, giving the same conclusion. The proof above establishes the needed cut statement directly.

## ↑ Ancestors (11)

1. [I](../i.md)
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
