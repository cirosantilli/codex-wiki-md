<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For [EM for zero-inflated negative binomial regression](../../../../../../em-for-zero-inflated-negative-binomial-regression.md), at iteration $k$ apply [Bayes' theorem](../../../../../../bayes-theorem.md) to each zero in the [zero-inflated negative binomial model](../../../../../../zero-inflated-negative-binomial-model.md). The E step computes the [conditional expectation](../../../../../../conditional-expectation.md) of its latent indicator:

$$
\boxed{t_i^{(k)}=\mathbb E[A_i\mid y_i]=\begin{cases}\displaystyle\frac{\pi^{(k)}}{\pi^{(k)}+(1-\pi^{(k)})(r/(r+\lambda_i^{(k)}))^r},&y_i=0,\\0,&y_i>0.\end{cases}}
$$

Treating these values as fixed, the M step maximizes the expected complete-data [log-likelihood](../../../../../../log-likelihood.md). Its two parameter blocks separate:

$$
\boxed{\pi^{(k+1)}=\frac1n\sum_i t_i^{(k)},\qquad \beta^{(k+1)}=\arg\max_\beta\sum_i w_i^{(k)}\log f_{\rm NB}(y_i;r,e^{x_i^T\beta}),\quad w_i^{(k)}=1-t_i^{(k)}.}
$$

The second block is a weighted [negative binomial regression](../../../../../../negative-binomial-regression.md) with fixed size $r$. Writing $\eta_i=x_i^T\beta$ and $\lambda_i=e^{\eta_i}$, its parameter-dependent objective is

$$
Q_\beta=\sum_iw_i\{y_i\eta_i-(y_i+r)\log(r+e^{\eta_i})\}.
$$

Its [score function](../../../../../../informant-function.md) and negative [Hessian matrix](../../../../../../hessian-matrix.md) are

$$
U(\beta)=\sum_iw_i\frac{r(y_i-\lambda_i)}{r+\lambda_i}x_i,\qquad -\nabla^2Q_\beta=\sum_iw_i\frac{r\lambda_i(y_i+r)}{(r+\lambda_i)^2}x_ix_i^T.
$$

The objective is [concave](../../../../../../concave-function.md), so a finite maximizer, when it exists, can be found by [Newton method](../../../../../../newton-s-method-in-optimization.md) or [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md). The latter uses working response $\eta_i+(y_i-\lambda_i)/\lambda_i$ and weights $w_i r\lambda_i/(r+\lambda_i)$. This is not an unweighted regression on only the positive counts: zeros retain fractional weight in the count component.

Start with $0<\pi<1$ and finite coefficients, alternate the two steps, and monitor the observed [log-likelihood](../../../../../../log-likelihood.md). Exact maximization makes the [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) nondecreasing in that likelihood, although the mixture may have multiple stationary points. All-zero data can lead to boundary fits and poor identification; multiple initializations and explicit checks for boundary parameters are useful.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
