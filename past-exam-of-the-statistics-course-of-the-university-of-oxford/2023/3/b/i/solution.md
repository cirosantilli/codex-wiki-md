<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Writing $s=\sum_i x_i$, the [Poisson distribution](../../../../../poisson-distribution.md) likelihood is proportional to $\theta^s e^{-n\theta}$. Multiplying by the [gamma distribution](../../../../../gamma-distribution.md) prior gives

$$
\pi(\theta\mid\boldsymbol x)\propto\theta^{r+s-1}e^{-(\lambda+n)\theta}.
$$

This is [Poisson-gamma conjugacy](../../../../../poisson-gamma-conjugacy.md), with the rate convention made explicit:

$$
\boxed{\theta\mid\boldsymbol x\sim\operatorname{Gamma}(r+s,\text{rate }\lambda+n)}.
$$

Its normalized density is $(\lambda+n)^{r+s}\theta^{r+s-1}e^{-(\lambda+n)\theta}/\Gamma(r+s)$ for $\theta>0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
