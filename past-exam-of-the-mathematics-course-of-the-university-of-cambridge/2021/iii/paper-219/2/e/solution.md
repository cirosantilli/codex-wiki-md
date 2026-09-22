<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The scale separation makes correlations between distinct observation times negligible, so $K_\theta\simeq A I$. Put $v_i=A+\sigma_i^2$. With a flat prior,

$$
\boxed{\mu\mid y,t,\theta\ \dot\sim\
N\left(\bar\mu,V_\mu\right)},\qquad
V_\mu=\left(\sum_i v_i^{-1}\right)^{-1},\quad
\bar\mu=V_\mu\sum_i\frac{y_i}{v_i}.
$$

The next latent value is likewise approximately independent of the past conditional on $\mu$, with $f_*\mid\mu\sim N(\mu,A)$. Marginalizing $\mu$ gives

$$
\boxed{f_*\mid y,t,\theta\ \dot\sim\ N(\bar\mu,A+V_\mu)}.
$$

When every $\sigma_i=0$, $\bar\mu=\bar y$, $V_\mu=A/N$, and the predictive variance is $A(1+1/N)$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
