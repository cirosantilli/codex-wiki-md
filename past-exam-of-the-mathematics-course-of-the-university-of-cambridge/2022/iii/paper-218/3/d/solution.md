<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Principal component analysis](../../../../../../principal-component-analysis.md) centers the word-count vectors, diagonalizes their sample [covariance matrix](../../../../../../covariance-matrix.md), and projects onto the eigenvectors with the largest eigenvalues. Fitting logistic regression to $d<n$ principal-component scores removes exact collinearity and yields a lower-dimensional design.

Each principal component is an unsupervised linear combination of many words chosen to explain predictor variance; it is not a word selected for association with spam. The dimension can be chosen from a scree plot or cumulative explained variance, but cross-validating the downstream classification loss better targets prediction.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
