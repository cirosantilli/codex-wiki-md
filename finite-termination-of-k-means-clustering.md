# Finite termination of K-means clustering

↑ **Parent:** [K-means clustering](k-means-clustering.md)

For a finite dataset, alternate nearest-centre assignment and replacement of each centre by the [centroid](centroid.md) of its assigned observations. Keep the current assignment whenever an observation is tied between nearest centres. A changed assignment then strictly decreases the within-cluster sum of squared [Euclidean distances](euclidean-distance.md); updating centres cannot increase it by the [centroid sum-of-squares identity](centroid-sum-of-squares-identity.md).

After each centre update, the centres are determined by the current [partition of a set](partition-of-a-set.md) of observation indices. There are only finitely many such partitions, so a strictly improving sequence cannot revisit one and must stop. A convenient exact stopping test is to check after each update whether every observation is still assigned to a nearest centre. This proof is for [algorithm termination](algorithm-termination.md); it does not guarantee a [global minimum](global-minimum.md).

Empty clusters need an explicit convention. To retain exactly $K\le n$ nonempty clusters, transfer an observation from a cluster with at least two members to each empty cluster, making it a singleton centred at that observation. This cannot increase the objective: the transferred observation now has squared distance zero, and no other contribution changes before centre updating. A deterministic choice is an eligible observation farthest from its currently assigned centre, with ties resolved by index. After the first round, an empty cluster can arise only during a strictly improving reassignment, so these repairs preserve the finite-termination argument.

## ↑ Ancestors (9)

1. [K-means clustering](k-means-clustering.md)
2. [Cluster analysis](cluster-analysis.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [One-dimensional K-means iteration bound](one-dimensional-k-means-iteration-bound.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-iii/9/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/undated/prelims/mathematics-iii-resit/8/a/solution.md)
