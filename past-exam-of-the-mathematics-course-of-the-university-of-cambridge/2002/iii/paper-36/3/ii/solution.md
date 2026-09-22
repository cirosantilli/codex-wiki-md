<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Poisson regression margin-matching score equations](../../../../../../poisson-regression-margin-matching-score-equations.md) from the site indicator for each $i\ge2$ directly give

$$
\sum_j e_{ij}=\sum_j y_{ij}\qquad(i=2,\ldots,8).
$$

Subtracting these seven row balances from the intercept equation $\sum_{ij}e_{ij}=\sum_{ij}y_{ij}$ gives the missing reference row balance. Therefore

$$
\boxed{\sum_j e_{ij}=\sum_j y_{ij}\quad\text{for every site }i}.
$$

The after-indicator score similarly gives $\sum_i e_{i2}=\sum_i y_{i2}$. Subtracting it from the intercept balance yields the before-column balance, so

$$
\boxed{\sum_i e_{ij}=\sum_i y_{ij}\quad(j=1,2)}.
$$

Thus the fitted before and after count totals are $114$ and $15$, and each fitted site total equals its observed total. These identities concern expected counts $e_{ij}=p_{ij}\widehat\mu_{ij}$; unequal exposures do not imply corresponding unweighted sums of fitted rates equal sums of observed rates. They follow from the unpenalized canonical Poisson [likelihood](../../../../../../likelihood-function.md) and the available intercept/factor columns, not from balanced exposure periods.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
