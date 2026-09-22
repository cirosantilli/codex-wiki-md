<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At fraction $0.8$, the [Lasso regularization path](../../../../../../lasso-regularization-path.md) lies between the vertical lines marked steps 4 and 5. In that interval the first five predictors have nonzero slopes: $X_1,X_2,X_4,X_5$ are positive and $X_3$ is negative. The sixth predictor remains at zero until the later part of the path, beyond this fraction. Therefore the chosen [Lasso](../../../../../../lasso.md) model includes

$$
\boxed{X_1,X_2,X_3,X_4,X_5\text{, with }X_6\text{ excluded}.}
$$

The [regression intercept](../../../../../../regression-intercept.md) is retained. In particular the negative $X_3$ trace has already left zero at fraction $0.8$; a small slope is not the same as a zero slope. The selected fraction came from ten-fold [K-fold cross-validation](../../../../../../k-fold-cross-validation.md), and is not a numerical value of the ridge penalty in the preceding parts.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
