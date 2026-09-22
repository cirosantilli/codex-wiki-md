<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The new [prior density](../../../../../../prior-density.md) contributes the factor $\lambda_i^{15}e^{-16\lambda_i}$. Multiplication by the [Poisson distribution](../../../../../../poisson-distribution.md) [likelihood](../../../../../../likelihood-function.md) gives

$$
\boxed{\lambda_i\mid y_i\sim\operatorname{Gamma}(y_i+16,E_i+16).}
$$

Its [posterior mean](../../../../../../posterior-mean.md) displays the resulting shrinkage:

$$
\mathbb E(\lambda_i\mid y_i)=\frac{y_i+16}{E_i+16}
=\frac{E_i}{E_i+16}\frac{y_i}{E_i}+\frac{16}{E_i+16}\cdot1.
$$

The observed risk ratio $y_i/E_i$ is pulled towards one, most strongly for small exposures. The [posterior variance](../../../../../../posterior-variance.md) is $(y_i+16)/(E_i+16)^2$.

## ↑ Ancestors (11)

1. [F](../f.md)
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
