<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply independent uniforms to the $n$ proposals, and let $I_i$ indicate acceptance. Each $I_i$ is Bernoulli with success probability $p=1/M$, and the indicators are independent because the pairs $(X_i,U_i)$ are independent. Hence

$$
\boxed{N=\sum_{i=1}^nI_i\sim\operatorname{Bin}(n,1/M),\qquad
\mathbb EN=\frac nM,\qquad\operatorname{Var}(N)=\frac nM\left(1-\frac1M\right).}
$$

For a fixed acceptance pattern, the values at accepted positions are independent with density $f$, by the single-trial conditional density calculation. The same product law holds for every pattern of a given size. Consequently, conditional on $N=m$, the ordered accepted observations have joint density $\prod_{j=1}^mf(y_j)$. This is the [binomial count and iid values in fixed-budget rejection sampling](../../../../../../binomial-count-and-iid-values-in-fixed-budget-rejection-sampling.md); the count provides no information about those target values.

There is a finite-sample empty-output event, with probability $(1-1/M)^n$. Any estimator dividing by $N$ must be defined separately on $N=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
