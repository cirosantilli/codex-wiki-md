<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The parameter-dependent part of the complete [multinomial distribution](../../../../../../../multinomial-distribution.md) [log-likelihood](../../../../../../../log-likelihood.md) is

$$
\ell_c(\theta)=y_1\log(1-\theta)+(y_2+y_3)\log\theta+C(y).
$$

The remaining probability factors and multinomial coefficient are constant in $\theta$. If $y_1+y_2+y_3>0$, differentiating gives $-y_1/(1-\theta)+(y_2+y_3)/\theta$, whose zero is

$$
\boxed{\widehat\theta=\frac{y_2+y_3}{y_1+y_2+y_3}.}
$$

The [log-likelihood](../../../../../../../log-likelihood.md) is concave. If $y_2+y_3=0<y_1$, its maximum is at zero; if $y_1=0<y_2+y_3$, its maximum is at one. These boundary cases are included by the same formula. If $y_1=y_2=y_3=0$, the data lie entirely in the parameter-independent fourth cell and every $\theta\in[0,1]$ is a [maximum-likelihood estimator](../../../../../../../maximum-likelihood-estimator.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
