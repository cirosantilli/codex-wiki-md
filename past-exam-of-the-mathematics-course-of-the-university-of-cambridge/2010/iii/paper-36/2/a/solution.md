<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the exposure $E_i$ as known and positive. The [Poisson distribution](../../../../../../poisson-distribution.md) [log-likelihood](../../../../../../log-likelihood.md), up to a parameter-independent constant, is $\ell_i(\lambda_i)=y_i\log\lambda_i-E_i\lambda_i$. Its first two derivatives are

$$
\ell_i'(\lambda_i)=\frac{y_i}{\lambda_i}-E_i,\qquad \ell_i''(\lambda_i)=-\frac{y_i}{\lambda_i^2}.
$$

Since $\mathbb E(Y_i)=E_i\lambda_i$, the [Fisher information](../../../../../../fisher-information-matrix.md) is

$$
\mathcal I_i(\lambda_i)=-\mathbb E\ell_i''(\lambda_i)=\frac{E_i}{\lambda_i}.
$$

The [Jeffreys prior](../../../../../../jeffreys-prior.md) is proportional to its square root. Removing the constant $\sqrt{E_i}$ gives

$$
\boxed{\pi_J(\lambda_i)\propto\lambda_i^{-1/2},\qquad\lambda_i>0.}
$$

This is an [improper prior](../../../../../../improper-prior.md): its integral diverges at infinity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
