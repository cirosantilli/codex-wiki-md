<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Among all depth-one [regression tree](../../../../../../regression-tree.md) splits, the best split separates the second observation from the first and third by cutting advert1 between $0.89$ and $1.13$. The test point with advert1 equal to zero reaches the leaf containing responses $60$ and $53$, so the output is their [arithmetic mean](../../../../../../arithmetic-mean.md),

$$
\widehat y=\frac{60+53}{2}=56.5.
$$

This [decision stump](../../../../../../decision-stump.md) makes a piecewise-constant prediction far outside the observed predictor range and cannot extrapolate the spending trend towards the origin. Its shallow structure and leaf averaging keep its [variance of an estimator](../../../../../../variance-of-an-estimator.md) modest, while that extrapolation failure can produce substantial [bias of an estimator](../../../../../../bias-of-an-estimator.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
