# Paired binary sample size calculation

↑ **Parent:** [McNemar's test](mcnemar-s-test.md)

For a paired binary difference $D=C-M$, set $\delta=P(C=1)-P(M=1)$ and $q=P(C\ne M)$. Then $\mathbb ED=\delta$ and $\operatorname{Var}(D)=q-\delta^2$. Under equal marginal probabilities the variance is $q$. The [McNemar test](mcnemar-s-test.md) has approximate upper rejection boundary $z_{1-\alpha/2}\sqrt{nq}$ for the sum of differences. Requiring that the alternative mean $n\delta$ exceed this boundary by $z_{1-\beta}\sqrt{n(q-\delta^2)}$ gives the displayed planning size for a positive alternative, neglecting its very small lower-tail rejection probability. Use $z_{1-\alpha}$ for a pre-specified one-sided test. The marginal probabilities alone do not determine $q$: co-occurrence of positive outcomes must be specified or bounded. Discreteness and [clustered data](clustered-data.md) can change achieved [statistical power](statistical-power.md).

## ↑ Ancestors (8)

1. [McNemar's test](mcnemar-s-test.md)
2. [Statistical hypothesis test](statistical-hypothesis-test.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-34/2/a/solution.md)
