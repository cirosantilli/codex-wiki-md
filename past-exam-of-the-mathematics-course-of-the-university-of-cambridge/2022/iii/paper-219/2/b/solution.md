<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $t_1<t_2<t_3$, the condition from part a becomes

$$
(t_3-t_1)^\eta
=(t_2-t_1)^\eta+(t_3-t_2)^\eta.
$$

It holds for arbitrary positive time gaps exactly when $\eta=1$. The resulting [exponential covariance function](../../../../../../exponential-covariance-function.md) is the covariance of a stationary [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md), hence has the [Markov property](../../../../../../markov-property.md).

Writing $a_{32}=e^{-(t_3-t_2)/\tau}$, the predictive law is

$$
y_3\mid y_2,y_1
\sim N\!\left(\mu+a_{32}(y_2-\mu),,1-a_{32}^2\right).
$$

As $t_3\to\infty$, $a_{32}\to0$, so the predictive mean tends to the stationary mean $\mu$ and the predictive variance tends to the stationary variance $1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
