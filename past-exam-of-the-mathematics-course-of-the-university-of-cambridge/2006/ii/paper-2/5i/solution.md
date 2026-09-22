<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

Independence and the Poisson [probabilities](../../../../../probability.md) give the log-likelihood

$$
\boxed{\ell(\beta)=\sum_{i=1}^n\left(Y_i\beta x_i-e^{\beta x_i}-\log(Y_i!)\right).}
$$

Its score and curvature are

$$
\ell'(\beta)=\sum_i x_i(Y_i-e^{\beta x_i}),\qquad \ell''(\beta)=-\sum_i x_i^2e^{\beta x_i}.
$$

If some $x_i\ne0$, this is [strictly concave](../../../../../strictly-concave-function.md). A finite maximum is therefore the unique zero of the score when such a zero exists. Newton iteration gives

$$
\boxed{\beta_{m+1}=\beta_m+\frac{\sum_i x_i(Y_i-e^{\beta_mx_i})}{\sum_i x_i^2e^{\beta_mx_i}}.}
$$

Start from a finite value, compute the score and curvature, and iterate until both the score and step are small. A line search that shortens a step until the [likelihood](../../../../../likelihood-function.md) increases improves robustness. [Strict concavity](../../../../../strict-concavity.md) identifies any converged [stationary point](../../../../../stationary-point.md) as the [global maximum](../../../../../global-maximum.md). A finite root need not exist, for example when all observations are zero and all $x_i>0$, in which case the [likelihood](../../../../../likelihood-function.md) supremum is at $\beta\to-\infty$. If all $x_i=0$, the parameter is unidentifiable.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
