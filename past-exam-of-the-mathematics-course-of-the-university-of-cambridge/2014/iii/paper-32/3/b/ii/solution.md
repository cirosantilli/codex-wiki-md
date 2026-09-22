<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply [MAR standardization over a fully observed covariate](../../../../../../../mar-standardization-over-a-fully-observed-covariate.md). All first-year statuses are known, so the estimated [probabilities](../../../../../../../probability.md) of no use and use in year one are $58/102$ and $44/102$. Within those categories, [missing at random](../../../../../../../missing-at-random.md) lets the observed second-year [probabilities](../../../../../../../probability.md) represent the corresponding dropout outcomes as well. They are estimated by $7/37$ and $18/28$.

The [law of total probability](../../../../../../../law-of-total-probability.md) then gives

$$
\boxed{\widehat P(Y_2=1)=\frac{58}{102}\frac7{37}+\frac{44}{102}\frac{18}{28}=0.384889\approx38.49\%.}
$$

Equivalently, impute expected drug-use counts $21(7/37)$ and $16(18/28)$ for the two dropout groups, add these to the 25 observed second-year users, and divide by 102. This uses both the complete records and the fully observed first-year information.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
