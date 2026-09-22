<h1 id="5j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Treat make as a categorical predictor, converting it to a factor explicitly if necessary:

`fit3 <- lm(log(price) ~ mpg + psngr + length + width + weight + factor(make), data = cars)`

The models are nested. The first [nested-model F-test](../../../../../../nested-model-f-test.md) compares fit2 with the intercept-only fit1. Adding the five quantitative predictors reduces the residual sum of squares from $8584.0$ to $3349.1$, with

$$
F=69.7334,\qquad p<2.2\times10^{-16}.
$$

There is overwhelming evidence that these quantitative car properties jointly improve the model.

The second test compares fit3 with fit2. Adding make reduces the residual sum of squares further to $840.8$, with

$$
F=5.3891,\qquad p=2.541\times10^{-8}.
$$

Thus manufacturer has a highly significant effect even after adjusting for the five quantitative properties, and fit3 is preferred among these nested models.

There are $93$ observations because the intercept-only model has $92=93-1$ residual degrees of freedom. The make term uses $31$ additional degrees of freedom. By the [degrees of freedom of a factor predictor](../../../../../../degrees-of-freedom-of-a-factor-predictor.md), a factor with $m$ represented levels contributes $m-1$ degrees of freedom when an intercept is present. Hence

$$
m-1=31,
\qquad
\boxed{m=32}
$$

unique manufacturers occur in the dataset.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5J](../../5j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
