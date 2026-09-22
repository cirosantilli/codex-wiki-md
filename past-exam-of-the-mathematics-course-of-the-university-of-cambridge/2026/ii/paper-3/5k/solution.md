<h1 id="5k/solution">Solution</h1>

↑ **Parent:** [5K](../5k.md)

The residual-versus-fitted [smooth curve](../../../../../smooth-curve.md) bends downward, indicating nonlinearity, and the spread increases at high fitted values. The Q-Q plot is close centrally but departs in both tails, with observations 12, 17, and 67 notable. The scale-location trend confirms heteroscedasticity. The leverage plot identifies observations 1 and 4 as high leverage and 67 as a large residual, with potentially material Cook distance. The additive Gaussian linear model is therefore doubtful. Inspect those observations, transform sale price (often logarithmically), add nonlinear or interaction terms and omitted predictors such as lot size and age, and use weighted or robust regression if unequal variance remains.

## ↑ Ancestors (10)

1. [5K](../5k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
