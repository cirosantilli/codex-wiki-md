<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [moral graph](../../../../../moral-graph.md) of a [Directed acyclic graph](../../../../../directed-acyclic-graph.md) is formed by joining any two parents of a common child and then removing the directions from all edges. For [D-separation](../../../../../d-separation.md), a path in the underlying undirected graph is active given $S$ when every noncollider on it is outside $S$, and every [collider](../../../../../collider.md) has itself or a descendant in $S$. Disjoint vertex sets $A$ and $B$ are [D-separated](../../../../../d-separation.md) by $S$ if no such active path connects them.

The adjacency characterization is

$$
\boxed{u,v\text{ are adjacent in the DAG}\quad\Longleftrightarrow\quad\text{no }S\subseteq V\setminus\{u,v\}\text{ d-separates them}.}
$$

A one-edge path cannot be blocked by conditioning on other vertices. For a nonadjacent pair, choose the later vertex $v$ in a [topological ordering](../../../../../topological-ordering.md). The earlier vertex $u$ is a nondescendant and is not a parent of $v$, so the parents of $v$ separate the pair by the [local Markov property of a directed acyclic graph](../../../../../local-markov-property-of-a-directed-acyclic-graph.md).

Use [faithfulness of a directed acyclic graph](../../../../../faithfulness-of-a-directed-acyclic-graph.md) to mean that graphical and probabilistic independences agree, for all disjoint sets:

$$
Z_A\perp Z_B\mid Z_S\quad\Longleftrightarrow\quad A\text{ and }B\text{ are d-separated by }S.
$$

This includes the [global Markov property of a directed acyclic graph](../../../../../global-markov-property-of-a-directed-acyclic-graph.md) as well as the absence of extra independences. The [conditional independence graph](../../../../../conditional-independence-graph.md) of $P$ is the undirected graph in which $u-v$ is absent exactly when $Z_u\perp Z_v\mid Z_{V\setminus\{u,v\}}$.

To identify this graph, condition on every vertex other than $u,v$. Any noncollider in the interior of a path is then conditioned on, so an active path must have only colliders internally. Two adjacent interior vertices cannot both be colliders: the arrow joining them has an arrowhead at only one of its ends. Thus an active path can have no interior vertex, giving a direct edge, or just one, giving $u\to w\leftarrow v$. In the latter case the conditioned common child $w$ activates the path. These possibilities are exactly the edges added or retained by moralization. Faithfulness therefore proves

$$
\boxed{\text{Moral graph of }\mathcal G=\text{conditional independence graph of }P.}
$$

This is why the [moral graph equals the conditional independence graph under faithfulness](../../../../../moral-graph-equals-the-conditional-independence-graph-under-faithfulness.md).

For Gaussian graph estimation, collect the data into an $n\times p$ matrix $D$ and let $S_n=n^{-1}\sum_i x_ix_i^T$. The [precision matrix](../../../../../precision-matrix.md) $\Theta=\Sigma^{-1}$ has $\Theta_{jk}=0$ precisely for absent graph edges, by [Gaussian conditional independence](../../../../../gaussian-conditional-independence.md). In [neighbourhood selection](../../../../../neighbourhood-selection.md), fit a [Lasso](../../../../../lasso.md) regression of each column on the others:

$$
\widehat b^{(j)}\in\arg\min_b\left\{\frac1{2n}\|D_j-D_{-j}b\|_2^2+\rho_j\|b\|_1\right\}.
$$

Select the nonzero coefficients as neighbours of $j$, then make the graph undirected using either the OR rule, retaining an edge selected in at least one regression, or the AND rule, requiring both. These are instances of [Nodewise Lasso](../../../../../nodewise-lasso.md).

The [Graphical Lasso](../../../../../graphical-lasso.md) estimates the whole precision matrix jointly, for example by

$$
\boxed{\widehat\Theta\in\arg\min_{\Theta\succ0}\left\{\operatorname{tr}(S_n\Theta)-\log\det\Theta+\rho\sum_{j\ne k}|\Theta_{jk}|\right\}.}
$$

Read off its nonzero off-diagonal entries as graph edges. This expression uses an off-diagonal penalty; an all-entry penalty is another convention.

To reduce computation in the [PC algorithm](../../../../../pc-algorithm.md), start its skeleton search from an estimate of the [conditional independence graph](../../../../../conditional-independence-graph.md) rather than the complete graph. The exact graph contains the true DAG skeleton, so oracle tests can remove its extra edges while retaining the true adjacencies. Fewer initial edges and smaller neighbourhoods reduce both candidate pairs and candidate conditioning sets.

For correctness of the orientation stage, preserve valid separating-set records. With an exact conditional independence graph, an initially absent pair $u,v$ has the full complement $V\setminus\{u,v\}$ as a separating set. Record that set, and record the usual discovered sets for edges removed later. Leaving an initially absent pair with an empty default could falsely mark an unshielded noncollider as a collider. This describes [PC initialization from a conditional independence graph](../../../../../pc-initialization-from-a-conditional-independence-graph.md); with an estimated initial graph, screening errors can propagate into the output.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
