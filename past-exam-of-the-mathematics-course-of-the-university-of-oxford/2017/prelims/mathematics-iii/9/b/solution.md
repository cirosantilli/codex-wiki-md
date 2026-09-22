<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $x_i\in\mathbb R^p$ for row $i$ of the [data matrix](../../../../../../data-matrix.md). The [k-means clustering](../../../../../../k-means-clustering.md) objective is the within-cluster sum of squared [Euclidean distances](../../../../../../euclidean-distance.md):

$$
\boxed{J(C_1,\ldots,C_K;m_1,\ldots,m_K)=\sum_{k=1}^K\sum_{i\in C_k}\|x_i-m_k\|^2.}
$$

The nonempty $C_k$ form a [partition of a set](../../../../../../partition-of-a-set.md) of observation indices. For fixed clusters, part (a) shows that the best $m_k$ is their [centroid](../../../../../../centroid.md).

Initialize distinct centres, for example by choosing $K\le n$ distinct observations. Then repeat the following steps:

- Assign each observation to a nearest centre in [Euclidean distance](../../../../../../euclidean-distance.md). Keep its current assignment on an exact tie; for a previously unassigned observation use a fixed ordering to resolve ties.
- If a cluster is empty, choose an observation from a cluster with at least two members and make it the empty cluster's sole member, placing its centre at that observation. A definite rule is to choose an eligible observation farthest from its currently assigned centre, breaking ties by observation index. Repeat until all clusters are nonempty.
- Replace each centre by the [arithmetic mean](../../../../../../arithmetic-mean.md) of its assigned observations.
- After updating, check whether every observation is still assigned to a nearest updated centre, retaining its assignment on ties. If so, stop; otherwise repeat.

The empty-cluster repair is possible for $K\le n$ and cannot increase $J$: the transferred observation now has squared distance zero, while all other squared distances stay unchanged before the centre update.

Assignment cannot increase $J$, and any changed assignment strictly decreases it under the tie rule. Updating centres cannot increase $J$ by the [centroid sum-of-squares identity](../../../../../../centroid-sum-of-squares-identity.md). After an update, the centres are determined by the [partition of a set](../../../../../../partition-of-a-set.md). There are only finitely many possible assignments. Unless this is the initial round, any nonterminal round starts with an assignment that strictly reduces $J$; repairing empty clusters and updating cannot undo that decrease. Thus a partition cannot recur, proving [finite termination of K-means clustering](../../../../../../finite-termination-of-k-means-clustering.md). The final result need not be a [global minimum](../../../../../../global-minimum.md); different initial centres can lead to different final clusterings.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
