# Maximum entropy distribution with a prescribed finite mean

↑ **Parent:** [Maximum entropy distribution on a finite set](maximum-entropy-distribution-on-a-finite-set.md)

For a finite list of real values $y_i$, maximize [information entropy](information-entropy-split.md) $H=-\sum_i p_i\log p_i$ with $p_i>0$, $\sum_i p_i=1$, and $\sum_i p_i y_i=Y$. [Lagrange multipliers](lagrange-multiplier.md) give

$$
p_i=\frac{e^{-by_i}}{Z(b)},\qquad
Z(b)=\sum_j e^{-by_j},\qquad
Y=-\frac{d}{db}\log Z(b).
$$

The constrained second variation is $-\sum_i(\delta p_i)^2/p_i<0$ for any nonzero tangent perturbation, proving uniqueness of the entropy maximum whenever a feasible interior solution exists. The mean has derivative $-\operatorname{Var}_b(y)$, so for nonconstant $y_i$ it decreases strictly with $b$ and ranges between the largest and smallest $y_i$ as $b$ ranges over the real line. Thus a finite $b$ exists uniquely exactly when $\min_i y_i<Y<\max_i y_i$.

At an extreme mean, strictly positive probabilities are impossible unless all $y_i$ coincide. If all $y_i=y_0$, the mean constraint is redundant when $Y=y_0$, the maximum is uniform, and $b$ is not identifiable. This finite [exponential family](exponential-family-split.md) is an [exponential tilting](exponential-tilting.md) of the uniform distribution.

## ↑ Ancestors (7)

1. [Maximum entropy distribution on a finite set](maximum-entropy-distribution-on-a-finite-set.md)
2. [Information entropy](information-entropy-split.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/19/c/solution.md)
