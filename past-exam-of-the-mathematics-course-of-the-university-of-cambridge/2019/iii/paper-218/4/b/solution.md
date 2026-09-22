<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fitted LDA rule replaces $\pi_l,\mu_l,\Sigma$ by class proportions, class sample means, and the pooled within-class covariance, then maximizes the resulting $\widehat\delta_l(x)$. Means and covariances have unbounded sensitivity, so a gross outlier can substantially move every LDA boundary. A soft-margin linear [support vector machine](../../../../../../support-vector-machine.md) uses hinge loss; observations beyond the correctly classified margin cease contributing, though mislabeled or extreme points can still matter according to the penalty $C$. Thus the SVM is generally more robust to well-classified extremes, while neither method is automatically robust to adversarial outliers.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
