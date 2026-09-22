<h1 id="13i/solution">Solution</h1>

↑ **Parent:** [13I](../13i.md)

The Gaussian log [likelihood function](../../../../../likelihood-function.md), apart from a constant, is

$$
\ell(\beta,\sigma^2)=-\frac n2\log\sigma^2-\frac{\|Y-X\beta\|^2}{2\sigma^2}.
$$

Differentiating in $\beta$ gives $X^{\mathsf T}(Y-X\widehat\beta)=0$. Full column rank makes $X^{\mathsf T}X$ invertible, so

$$
\boxed{\widehat\beta=(X^{\mathsf T}X)^{-1}X^{\mathsf T}Y,\qquad
\widehat\beta\sim N_p(\beta,\sigma^2(X^{\mathsf T}X)^{-1})}.
$$

The distribution follows by applying this linear map to the Gaussian error vector. Differentiating the profiled [likelihood function](../../../../../likelihood-function.md) in $\sigma^2$ gives

$$
\boxed{\widehat\sigma^2=\frac1n\|Y-X\widehat\beta\|^2}.
$$

For its distribution, $P=X(X^{\mathsf T}X)^{-1}X^{\mathsf T}$ is symmetric idempotent, and the residual is $(I-P)\epsilon$. The needed form of [Cochran's theorem](../../../../../cochran-s-theorem.md) says that quadratic forms in a standard Gaussian vector associated with orthogonal symmetric projection matrices summing to identity are independent random variables with [chi-squared distributions](../../../../../chi-squared-distribution.md) with degrees equal to their ranks. Applying it to $P$ and $I-P$ gives

$$
\boxed{\frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-p}}.
$$

Thus the maximum-likelihood variance estimate uses divisor $n$ and has expectation $(n-p)\sigma^2/n$; the unbiased residual estimate would use divisor $n-p$. The fitted coefficient and residual quadratic form are also independent.

## ↑ Ancestors (10)

1. [13I](../13i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
