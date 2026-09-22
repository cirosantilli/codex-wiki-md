<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For observations $\mathbf x_i\in\mathbb R^p$, [K-means clustering](../../../../../../k-means-clustering.md) seeks nonempty [clusters in cluster analysis](../../../../../../cluster-in-cluster-analysis.md) $C_1,\ldots,C_K$ and [centroids](../../../../../../centroid.md) $\mathbf m_k$ minimizing

$$
\boxed{W=\sum_{k=1}^K\sum_{i\in C_k}\|\mathbf x_i-\mathbf m_k\|^2,\qquad
\mathbf m_k=\frac1{|C_k|}\sum_{i\in C_k}\mathbf x_i.}
$$

At fixed [centroids](../../../../../../centroid.md), assigning each point to a nearest [centroid](../../../../../../centroid.md) minimizes its squared [Euclidean distance](../../../../../../euclidean-distance.md). At fixed assignments, the [centroid sum-of-squares identity](../../../../../../centroid-sum-of-squares-identity.md) shows that the [sample mean](../../../../../../sample-mean.md) uniquely minimizes each group's contribution. These alternating steps cannot increase $W$.

For [finite termination of K-means clustering](../../../../../../finite-termination-of-k-means-clustering.md), more than a lower bound on $W$ is needed. Keep an assignment unchanged when nearest [centroids](../../../../../../centroid.md) tie, and stop when assignments no longer change. Every change then strictly decreases $W$. After updating the [centroids](../../../../../../centroid.md), $W$ is determined by the [partition of a set](../../../../../../partition-of-a-set.md) of $n$ indices; there are only finitely many choices for that [partition of a set](../../../../../../partition-of-a-set.md), so no strictly improving [partition of a set](../../../../../../partition-of-a-set.md) can recur. Empty [clusters in cluster analysis](../../../../../../cluster-in-cluster-analysis.md) require a convention, such as moving a point from a nonsingleton [cluster in cluster analysis](../../../../../../cluster-in-cluster-analysis.md) to become its own [centroid](../../../../../../centroid.md), which cannot increase $W$. With such a consistent convention the algorithm terminates, although it may reach only a [local minimum](../../../../../../local-minimum.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Mathematics III resit](../../../mathematics-iii-resit-split.md)
4. [Prelims](../../../split.md)
5. [Undated](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
