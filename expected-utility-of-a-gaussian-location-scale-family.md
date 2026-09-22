# Expected utility of a Gaussian location-scale family

↑ **Parent:** [Expected utility maximization](expected-utility-maximization.md)

For $X=\mu+\sigma Z$ with $Z$ having the [standard normal distribution](standard-normal-distribution.md) and an increasing concave [utility function](utility-function-split.md) $U$, define $f(\mu,\sigma)=\mathbb E[U(X)]$. Then $f_\mu=\mathbb E[U'(X)]>0$ and [Gaussian integration by parts](stein-s-lemma-probability.md) gives $f_\sigma=\sigma\mathbb E[U''(X)]\leq0$. Moreover

$$
\operatorname{Hess}f
=\mathbb E\left[U''(X)
\begin{pmatrix}1&Z\\Z&Z^2\end{pmatrix}\right]
$$

is negative semidefinite, so $f$ is jointly [concave](concave-function.md) in $\mu$ and $\sigma$.

## ↑ Ancestors (8)

1. [Expected utility maximization](expected-utility-maximization.md)
2. [Expected utility hypothesis](expected-utility-hypothesis.md)
3. [Utility function](utility-function-split.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
