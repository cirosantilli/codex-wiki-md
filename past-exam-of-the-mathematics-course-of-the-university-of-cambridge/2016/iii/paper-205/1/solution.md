<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $V=\{1,\ldots,p\}$. The [global Markov property for a directed acyclic graph](../../../../../global-markov-property-for-a-directed-acyclic-graph.md) says that, for every three pairwise disjoint vertex sets $A,B,C$,

$$
A\text{ and }B\text{ are D-separated by }C\text{ in }\mathcal G\quad\Longrightarrow\quad Z_A\mathrel{\perp\!\!\!\perp}Z_B\mid Z_C.
$$

Thus graphical [D-separation](../../../../../d-separation.md) implies probabilistic [conditional independence](../../../../../conditional-independence.md). [Causal minimality](../../../../../causal-minimality.md) means that $P$ has this [global Markov property for a directed acyclic graph](../../../../../global-markov-property-for-a-directed-acyclic-graph.md), but has it for no proper subgraph of $\mathcal G$ obtained by deleting edges while keeping all vertices. [Faithfulness of a directed acyclic graph](../../../../../faithfulness-of-a-directed-acyclic-graph.md) means that the displayed implication is an equivalence: the [conditional independences](../../../../../conditional-independence.md) of $P$ are exactly the [D-separations](../../../../../d-separation.md) of $\mathcal G$. In particular it includes the [global Markov property for a directed acyclic graph](../../../../../global-markov-property-for-a-directed-acyclic-graph.md).

**A causally minimal distribution can nevertheless have an extra independence.** Here is a [causally minimal nonfaithful Gaussian model](../../../../../causally-minimal-nonfaithful-gaussian-model.md). Take three [independent random variables](../../../../../independent-random-variables.md) $E_1,E_2,E_3$, each with the [standard normal distribution](../../../../../standard-normal-distribution.md), and set

$$
Z_1=E_1,\qquad Z_2=Z_1+E_2,\qquad Z_3=Z_2-Z_1+E_3.
$$

Use the [Directed acyclic graph](../../../../../directed-acyclic-graph.md) with edges $1\to2$, $1\to3$ and $2\to3$. The equations give a [directed acyclic graph factorization](../../../../../directed-acyclic-graph-factorization.md), so the [global Markov property for a directed acyclic graph](../../../../../global-markov-property-for-a-directed-acyclic-graph.md) holds. Alternatively this complete acyclic graph imposes no nontrivial [D-separations](../../../../../d-separation.md). But $Z_3=E_2+E_3$ is [independent](../../../../../independent-random-variables.md) of $Z_1=E_1$, even though the direct edge $1\to3$ prevents their [D-separation](../../../../../d-separation.md). Hence [faithfulness of a directed acyclic graph](../../../../../faithfulness-of-a-directed-acyclic-graph.md) fails.

To check [causal minimality](../../../../../causal-minimality.md) explicitly, the [covariance matrix](../../../../../covariance-matrix.md) is

$$
\Sigma=\begin{pmatrix}1&1&0\\1&2&1\\0&1&2\end{pmatrix}.
$$

The linear transformation from $(E_1,E_2,E_3)$ to $(Z_1,Z_2,Z_3)$ is invertible, so this is a nonsingular [multivariate normal distribution](../../../../../multivariate-normal-distribution.md). Deleting $1\to2$ would require $Z_1\perp Z_2$, whereas $\operatorname{Cov}(Z_1,Z_2)=1$. Deleting $1\to3$ would require $Z_1\perp Z_3\mid Z_2$, whereas the conditional [covariance](../../../../../covariance.md) is

$$
\operatorname{Cov}(Z_1,Z_3\mid Z_2)=0-\frac{1\cdot1}{2}=-\frac12.
$$

Deleting $2\to3$ would require $Z_2\perp Z_3\mid Z_1$, whereas its conditional [covariance](../../../../../covariance.md) is $1-1\cdot0=1$. By [Gaussian conditional independence](../../../../../gaussian-conditional-independence.md), each nonzero conditional [covariance](../../../../../covariance.md) rules out the required independence. Every proper subgraph is contained in a graph obtained by a single edge deletion, and further deletion can only add Markov restrictions. Thus no proper subgraph is Markov for $P$, proving [causal minimality](../../../../../causal-minimality.md).

For the [Markov blanket](../../../../../markov-blanket.md), use its standard convention that the focal vertex is excluded:

$$
B=\operatorname{mb}(k)=\bigl(\operatorname{pa}(k)\cup\operatorname{ch}(k)\cup\operatorname{pa}(\operatorname{ch}(k))\bigr)\setminus\{k\}.
$$

We prove [Markov blanket D-separation](../../../../../markov-blanket-d-separation.md) by examining an arbitrary path from $k$ to $v\notin B\cup\{k\}$. If its first edge points into $k$, its next vertex is a parent of $k$, hence a conditioned noncollider in $B$, and the path is blocked. Otherwise the path starts $k\to h$ at a child $h\in B$. If the next edge points out of $h$, then $h$ is again a conditioned noncollider. If it points into $h$, the path begins $k\to h\leftarrow u$. Although conditioning on the [collider](../../../../../collider.md) $h$ opens that local segment, $u$ is another parent of $h$, hence belongs to $B$. The outgoing arrow $u\to h$ makes $u$ a noncollider on the path, so conditioning on $u$ blocks it. Since $v$ is outside $B$, none of these blocking vertices can be the endpoint.

Every path is therefore blocked by $B$. Applying the [global Markov property for a directed acyclic graph](../../../../../global-markov-property-for-a-directed-acyclic-graph.md) gives

$$
\boxed{Z_k\mathrel{\perp\!\!\!\perp}Z_{V\setminus(B\cup\{k\})}\mid Z_B.}
$$

This proves the requested screening property without any positivity assumption on $P$.

Finally assume [faithfulness of a directed acyclic graph](../../../../../faithfulness-of-a-directed-acyclic-graph.md) and let $A$ have the stated screening property. Then $k$ and every vertex outside $A\cup\{k\}$ must be [D-separated](../../../../../d-separation.md) by $A$. If a parent or child $h$ of $k$ were missing from $A$, the one-edge path between them would be active, a contradiction. Thus every parent and child is in $A$. If another parent $u$ of a child $h$ were missing from $A$, the path $k\to h\leftarrow u$ would be active: its only interior vertex is the [collider](../../../../../collider.md) $h$, already in $A$. This is again a contradiction. Consequently

$$
\boxed{A\supseteq\operatorname{mb}(k).}
$$

**Under faithfulness the graphical blanket is contained in every screening set.** This is the [minimal Markov blanket under faithfulness](../../../../../minimal-markov-blanket-under-faithfulness.md); the preceding argument also shows that the blanket itself is a screening set.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
