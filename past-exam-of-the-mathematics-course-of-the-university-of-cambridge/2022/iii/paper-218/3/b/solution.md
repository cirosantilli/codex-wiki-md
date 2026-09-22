<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [decision boundary](../../../../../../decision-boundary.md) is the hyperplane

$$
\widehat\beta_0+x^T\widehat\beta=0.
$$

At threshold $q$ the classifier predicts spam when

$$
\widehat\beta_0+x^T\widehat\beta
>\log\frac q{1-q},
$$

so $q=1/2$ gives the original classifier. Varying $q$ translates the boundary parallel to itself: raising $q$ shrinks the region classified as spam and generally trades fewer false positives for more false negatives.

## ↑ Ancestors (11)

1. [B](../b.md)
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
