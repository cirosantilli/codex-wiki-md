<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The loop performs [Leave-one-out cross-validation](../../../../../../leave-one-out-cross-validation.md): for each $i$ it fits a forest to the other eight observations, tests it on observation $i$, and averages the nine zero-one losses. A random forest's [out-of-bag error estimate](../../../../../../out-of-bag-error.md) approximates the same held-out prediction error from one fit, because each tree automatically omits roughly a proportion $e^{-1}$ of the observations in its [bootstrap sample](../../../../../../bootstrap-sample.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
