<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

Let $M=\min_i x_i$ and $S=\sum_i(x_i-M)$. On the likelihood support $0<\mu\le M$, the log likelihood is $n\log\lambda-\lambda\sum_i(x_i-\mu)$. For fixed $\lambda$ it increases with $\mu$, so $\hat\mu=M$. Maximizing in $\lambda$ then gives the [shifted exponential maximum likelihood](../../../../../shifted-exponential-maximum-likelihood.md) estimates

$$
\boxed{\hat\mu=M,\qquad\hat\lambda=n/S,\qquad
\hat\beta=M+S/n=\overline x.}
$$

These finite estimates exist almost surely for $n\ge2$. For one observation, or an all-equal sample, the likelihood is unbounded as $\lambda\to\infty$.

The minimum has $M-\mu\sim\operatorname{Exp}(n\lambda)$, so $E\hat\mu=\mu+1/(n\lambda)$: its bias is positive. By exponential memorylessness, $S\sim\operatorname{Gamma}(n-1,\text{rate }\lambda)$. For $n>2$, integration of the gamma density gives $E(1/S)=\lambda/(n-2)$, and hence

$$
\boxed{E\hat\lambda=\frac{n\lambda}{n-2},\quad
\operatorname{bias}(\hat\lambda)=\frac{2\lambda}{n-2}>0.}
$$

At $n=2$ this inverse moment is infinite, so a finite bias does not exist. Finally $E\overline X=\mu+1/\lambda=\beta$, so **$\hat\beta$ is unbiased**. The positivity assertions are therefore subject to the sample-size qualifications above.

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
