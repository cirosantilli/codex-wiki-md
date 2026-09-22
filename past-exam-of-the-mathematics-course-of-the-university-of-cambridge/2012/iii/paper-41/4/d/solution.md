<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Only sets 4, 5, 7 and 8 have an earlier failure with both members at risk. Sets 4 and 8 have B fail first and favor A, giving $6+3=9$ informative pairs. Sets 5 and 7 have A fail first and favor B, giving $18+9=27$. Both-censored pairs contribute zero; in sets 3 and 6 the earlier observation is censoring, so the later failure occurs with no remaining comparator and also contributes zero.

There are thus 36 informative independent strata. The [stratified log-rank statistic](../../../../../../stratified-log-rank-statistic.md), its null [variance](../../../../../../variance-split.md), and its standardized value are

$$
\boxed{U_A=(27-9)/2=9,\qquad V=36/4=9,\qquad Z=U_A/\sqrt V=3.}
$$

Equivalently the squared statistic is nine. The [normal approximation](../../../../../../normal-approximation.md) gives a two-sided [p-value](../../../../../../p-value.md) $2[1-\Phi(3)]<0.0027$ using the stated bound. The exact conditional [sign test](../../../../../../sign-test.md) instead gives $2\sum_{k=0}^{9}\binom{36}{k}2^{-36}\approx0.00393$; the slight difference is discreteness rather than a different direction of effect. **There is strong evidence favoring Method B**, which is associated with the later failure in three quarters of the informative pairs, under the test assumptions.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
