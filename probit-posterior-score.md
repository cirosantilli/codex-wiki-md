# Probit posterior score

↑ **Parent:** [Probit model](probit-model.md)

For [probit regression](probit-model.md) with $s_i=2Y_i-1$ and prior $N(0,\sigma^2I)$, the [posterior score control variate](posterior-score-control-variate.md) is

$$
g(\beta)=-\frac\beta{\sigma^2}+\sum_i s_ix_i\frac{\phi(s_ix_i^T\beta)}{\Phi(s_ix_i^T\beta)}.
$$

For $h(\beta)=\Phi(x_*^T\beta)$, its covariance with the score is $-x_*\mathbb E[\phi(x_*^T\beta)]$. It is nonzero whenever $x_*\ne0$, ensuring strict improvement by the optimal [control variate](control-variates.md).

## ↑ Ancestors (8)

1. [Probit model](probit-model.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/6/b/solution.md)
