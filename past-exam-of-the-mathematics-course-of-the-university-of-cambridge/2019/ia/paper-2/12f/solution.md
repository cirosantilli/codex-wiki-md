<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

Let $X_i=\mathbf1_{A_i}$ be the [indicator random variable](../../../../../indicator-random-variable.md) of $A_i$. Then $X=\sum_iX_i$, so [linearity of expectation](../../../../../linearity-of-expectation.md) gives

$$
\boxed{\mathbb E X=\sum_{i=1}^n\mathbb E X_i=\sum_{i=1}^n\mathbb P(A_i)}.
$$

Using [variance of a sum](../../../../../variance-of-a-sum.md) and

$$
\operatorname{Cov}(X_i,X_j)
=\mathbb E(X_iX_j)-\mathbb E X_i\mathbb E X_j
=\mathbb P(A_i\cap A_j)-\mathbb P(A_i)\mathbb P(A_j),
$$

we obtain

$$
\boxed{\operatorname{Var}(X)=\sum_{i=1}^n\sum_{j=1}^n
\left[\mathbb P(A_i\cap A_j)-\mathbb P(A_i)\mathbb P(A_j)\right]}.
$$

For the circular array, let $X_i$ indicate that bulbs $i$ and $i+1$ are both on, with indices read modulo $n$. Then $\mathbb E X_i=p^2$. Non-neighbouring indicators are independent, while

$$
\operatorname{Var}(X_i)=p^2-p^4,
\qquad
\operatorname{Cov}(X_i,X_{i+1})=p^3-p^4.
$$

There are $n$ individual terms and $2n$ ordered neighbouring pairs in the double covariance sum, so

$$
\boxed{\mathbb E X=np^2},
\qquad
\boxed{\operatorname{Var}(X)=n(p^2+2p^3-3p^4)}.
$$

The event $B$ is exactly $\{X\geq1\}$. If $p=n^{-0.6}$, [Markov inequality](../../../../../markov-inequality.md) gives

$$
\mathbb P(B)\leq\mathbb E X=np^2=n^{-0.2}\longrightarrow0.
$$

If $p=n^{-0.4}$, then $B^c=\{X=0\}$ implies $|X-\mathbb EX|\geq\mathbb EX$. By [Chebyshev inequality](../../../../../chebyshev-inequality.md),

$$
\mathbb P(B^c)\leq\frac{\operatorname{Var}(X)}{(\mathbb EX)^2}
=\frac1{np^2}+\frac2{np}-\frac3n
=n^{-0.2}+2n^{-0.6}-3n^{-1}\longrightarrow0.
$$

Therefore $\boxed{\mathbb P(B)\to1}$ in the second regime.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
