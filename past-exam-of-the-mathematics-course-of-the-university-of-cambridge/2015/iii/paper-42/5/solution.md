<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use positive ability parameters in the [Bradley-Terry model](../../../../../bradley-terry-model.md), so $\mathbb P(i\text{ beats }j)=\theta_i/(\theta_i+\theta_j)$. If the course instead denotes log abilities by $\theta_i$, apply the following calculation to their exponentials; the ordering is unchanged. Up to a factor independent of the abilities, the [likelihood function](../../../../../likelihood-function.md) is

$$
L(\theta)=\frac{\theta_1}{\theta_1+\theta_2}
\frac{\theta_3}{\theta_1+\theta_3}
\left(\frac{\theta_2}{\theta_2+\theta_3}\right)^k.
$$

The observed wins form a directed cycle, so a finite maximum exists. The [Bradley-Terry likelihood Hessian](../../../../../bradley-terry-likelihood-hessian.md) is negative definite on contrasts of log abilities, giving uniqueness up to common scaling. We can therefore find the [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) through the [Bradley-Terry score equations](../../../../../bradley-terry-score-equation.md).

Player 1 has one observed win in two comparisons. Its score equation is

$$
1=\frac{\theta_1}{\theta_1+\theta_2}
+\frac{\theta_1}{\theta_1+\theta_3},
$$

which simplifies to $\theta_1^2=\theta_2\theta_3$. By the model's scale invariance, set $\theta_2=1$ and write $\theta_1=r$, $\theta_3=r^2$, with $r>0$. Player 2's score equation becomes

$$
k=\frac1{1+r}+\frac{k}{1+r^2},
\qquad kr^3+(k-1)r^2=1.
$$

The left side of the polynomial equation is strictly increasing on $r>0$, starts at zero, and tends to infinity. For $k=1$, its unique solution is $r=1$. For $k>1$, its value at one is $2k-1>1$, so its solution satisfies $0<r<1$. The [Three-player Bradley-Terry comparison cycle](../../../../../three-player-bradley-terry-comparison-cycle.md) consequently gives

$$
\boxed{k=1:\quad\widehat\theta_1=\widehat\theta_2=\widehat\theta_3;
\qquad k>1:\quad\widehat\theta_2>\widehat\theta_1>\widehat\theta_3.}
$$

Thus there is a complete tie when each directed edge is observed once, and otherwise the decreasing ranking is **2, 1, 3**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
