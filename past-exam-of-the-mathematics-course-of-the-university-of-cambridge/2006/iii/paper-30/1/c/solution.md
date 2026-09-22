<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $N\sim\operatorname{Pois}(\lambda)$, the [Poisson distribution](../../../../../../poisson-distribution.md) gives

$$
H(N)=\lambda\log_2e-\lambda\log_2\lambda+\mathbb E\log_2(N!).
$$

This [information entropy](../../../../../../information-entropy.md) is finite: $\log_2(n!)\leq n^2$ for integer $n\geq0$, while $\mathbb E N^2=\lambda+\lambda^2$.

Fix $0<\lambda_1<\lambda_2$. Take [independent random variables](../../../../../../independent-random-variables.md) $U\sim\operatorname{Pois}(\lambda_1)$ and $V\sim\operatorname{Pois}(\lambda_2-\lambda_1)$. Their [convolution](../../../../../../convolution.md) is

$$
\mathbb P(U+V=n)
=e^{-\lambda_2}\sum_{j=0}^n
\frac{\lambda_1^j(\lambda_2-\lambda_1)^{n-j}}{j!(n-j)!}
=e^{-\lambda_2}\frac{\lambda_2^n}{n!},
$$

by the [binomial theorem](../../../../../../binomial-theorem.md). Thus $U+V$ has [Poisson distribution](../../../../../../poisson-distribution.md) with parameter $\lambda_2$. Conditioning on $V=v$ only translates $U$, so $H(U+V\mid V)=H(U)=F(\lambda_1)$. The [entropy monotonicity under independent addition](../../../../../../entropy-monotonicity-under-independent-addition.md) yields $F(\lambda_2)\geq F(\lambda_1)$.

In fact the inequality is strict. The [covariance](../../../../../../covariance.md) $\operatorname{Cov}(U+V,V)=\operatorname{Var}(V)=\lambda_2-\lambda_1$ is positive, so $U+V$ and $V$ are not [independent random variables](../../../../../../independent-random-variables.md). Their [information entropies](../../../../../../information-entropy.md) are finite, and the equality criterion from part (a) excludes equality. Therefore the [Poisson entropy monotonicity](../../../../../../poisson-entropy-monotonicity.md) gives the stronger conclusion

$$
\boxed{\lambda_2>\lambda_1>0\ \Longrightarrow\ F(\lambda_2)>F(\lambda_1).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
