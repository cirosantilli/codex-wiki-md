<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $M\in\{1,2\}$ be one fixed model indicator with equal prior probabilities, and put $w_{m,t}=\mathbb P(M=m\mid y_1,\ldots,y_{t-1})$. Within each model the parameters are already updated using the same past data. The [Bayesian model averaging](../../../../../../bayesian-model-averaging.md) forecast is $f_t(y)=\sum_mw_{m,t}f_{mt}(y)$. Upon observing $y_t$, [Bayes' theorem](../../../../../../bayes-theorem.md) gives

$$
\boxed{w_{m,t+1}
=\frac{w_{m,t}f_{mt}(y_t)}
{\sum_jw_{j,t}f_{jt}(y_t)}.}
$$

Taking the ratio cancels the denominator and gives the prescribed update because $f_{mt}(y_t)=e^{L_{mt}}$. Iteration yields

$$
\boxed{\frac{w_{1,T+1}}{w_{2,T+1}}=e^{T_1-T_2}=B_{12}.}
$$

The weights are posterior model probabilities and their mixture is the full Bayesian predictive density. The indicator is fixed across days, rather than choosing a fresh model independently each morning.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
