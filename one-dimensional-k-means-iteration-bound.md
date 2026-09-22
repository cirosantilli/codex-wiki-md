# One-dimensional K-means iteration bound

↑ **Parent:** [K-means clustering](k-means-clustering.md)

For $n$ distinct observations on the real line and $1\le K\le n$, nearest-centre assignment produces contiguous blocks of the sorted observations because each [Voronoi cell](voronoi-cell.md) is an [interval](interval-mathematics.md). The [arithmetic means](arithmetic-mean.md) of distinct ordered blocks are strictly ordered, preserving this property at subsequent assignments. Initialize at $K$ distinct observed values so that the initial assignment has no empty cluster.

The empty-cluster repair in [finite termination of K-means clustering](finite-termination-of-k-means-clustering.md) also preserves contiguous blocks: an observation farthest from a centre over its assigned block lies at one of that block's endpoints, so transferring it to a new singleton splits the block into two contiguous blocks.

There are $\binom{n-1}{K-1}$ possible partitions into $K$ nonempty blocks: choose $K-1$ cuts among the $n-1$ gaps. Under the stable tie rule in [finite termination of K-means clustering](finite-termination-of-k-means-clustering.md), every round after the first strictly reduces the objective until stopping, so a block partition cannot recur. The number of assignment, repair, and centre-update rounds is therefore at most $\binom{n-1}{K-1}\le n^{K-1}$. Check stability after each update without an additional update round; for $K=1$, one update suffices.

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

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-iii/9/c/solution.md)
