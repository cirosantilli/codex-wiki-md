<h1 id="30j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write

$$
\bar X_m=\frac1m\sum_{i=1}^mX_i,
\qquad
\bar Y_m=\frac1m\sum_{i=1}^mY_i.
$$

The [ordinary least squares estimators](../../../../../../ordinary-least-squares-estimators.md) give

$$
\widehat f_m(x)=\widehat\alpha_m+\widehat\beta_mx
=\bar Y_m+\widehat\beta_m(x-\bar X_m),
$$

where

$$
\widehat\beta_m
=\frac{\sum_{i=1}^m(X_i-\bar X_m)(Y_i-\bar Y_m)}
{\sum_{i=1}^m(X_i-\bar X_m)^2}
=\frac{\sum_{i=1}^mX_iY_i-m\bar X_m\bar Y_m}
{\sum_{i=1}^mX_i^2-m\bar X_m^2}.
$$

The denominator is positive because the sorted inputs are distinct and $m\geq2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
