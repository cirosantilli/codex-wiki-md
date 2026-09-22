<h1 id="13j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write

$$
Y=\mu+\varepsilon,
\qquad
Y^*=\mu+\varepsilon^*,
$$

where $\varepsilon$ and $\varepsilon^*$ are independent, centered, and have covariance matrix $\sigma^2I_n$. Then

$$
HY-Y^*=-(I-H)\mu+H\varepsilon-\varepsilon^*.
$$

The deterministic term is orthogonal in expectation to the two centered random terms, and the random terms are independent. Since the [hat matrix](../../../../../../hat-matrix.md) is a symmetric idempotent projection of rank $p$,

$$
\mathbb E\|H\varepsilon\|^2
=\sigma^2\operatorname{tr}(H^TH)
=\sigma^2\operatorname{tr}H=p\sigma^2,
$$

while $\mathbb E\|\varepsilon^*\|^2=n\sigma^2$. Therefore

$$
\boxed{
\mathbb E\|HY-Y^*\|^2
=\|(I-H)\mu\|^2+(n+p)\sigma^2
}.
$$

In this [bias-variance decomposition for linear prediction](../../../../../../bias-variance-decomposition-for-linear-prediction.md), $\|(I-H)\mu\|^2$ is squared model bias, $p\sigma^2$ is variance from fitting $p$ coefficients, and $n\sigma^2$ is irreducible noise in the future response. Enlarging the model tends to reduce the first term while increasing the fitted-model variance, which is the bias-variance tradeoff.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
