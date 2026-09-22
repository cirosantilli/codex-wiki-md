# Classical multidimensional scaling

↑ **Parent:** [Multidimensional scaling](multidimensional-scaling.md)

For a symmetric zero-diagonal [dissimilarity matrix](dissimilarity-matrix.md) $D$, square each entry to obtain $D^{(2)}$ and put $H=I-\mathbf1\mathbf1^T/n$. Take the [eigenvectors](eigenvector.md) of $G=-HD^{(2)}H/2$ corresponding to its largest positive [eigenvalues](eigenvalue.md). Multiplying them by square roots of these [eigenvalues](eigenvalue.md) gives coordinates. If $D$ contains [Euclidean distances](euclidean-distance.md), $G$ is a centered [Gram matrix](gram-matrix.md), so retaining all positive [eigenvalues](eigenvalue.md) reconstructs those distances exactly. Retaining fewer approximates the [Gram matrix](gram-matrix.md), not generally the sum of squared errors in raw distances. Negative [eigenvalues](eigenvalue.md) signal failure of an exact Euclidean representation. Coordinates are unchanged in meaning by [orthogonal transformations](orthogonal-transformation.md).

**Table of contents**

- [Euclidean distance matrix criterion](euclidean-distance-matrix-criterion.md)

## ↑ Ancestors (9)

1. [Multidimensional scaling](multidimensional-scaling.md)
2. [Unsupervised learning](unsupervised-learning.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Multidimensional scaling](multidimensional-scaling.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43/4/solution.md)
