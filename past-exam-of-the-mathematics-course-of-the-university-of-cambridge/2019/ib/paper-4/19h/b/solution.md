<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For this model, the [Gauss-Markov theorem](../../../../../../gauss-markov-theorem.md) states that $\widehat\beta$ is the unique minimum-variance [linear unbiased estimator](../../../../../../linear-unbiased-estimator.md) of $\beta$: if

$$
\widetilde\beta=\sum_{i=1}^n a_iY_i
$$

is unbiased for every $\beta$, then $\operatorname{var}(\widetilde\beta)\geq\operatorname{var}(\widehat\beta)$.

Indeed,

$$
\mathbb E\widetilde\beta
=\beta\sum_i a_ix_i,
$$

so unbiasedness is equivalent to $\sum_i a_ix_i=1$. Write

$$
a_i=\frac{x_i}{S_{xx}}+c_i.
$$

The constraint becomes $\sum_i c_ix_i=0$. Since the errors are [independent](../../../../../../independent-random-variables.md) with common variance $\sigma^2$,

$$
\begin{aligned}
\operatorname{var}(\widetilde\beta)
&=\sigma^2\sum_i a_i^2\\
&=\sigma^2\left(\frac1{S_{xx}}+\frac2{S_{xx}}\sum_i c_ix_i+\sum_i c_i^2\right)\\
&=\frac{\sigma^2}{S_{xx}}+\sigma^2\sum_i c_i^2\\
&\geq\frac{\sigma^2}{S_{xx}}
=\operatorname{var}(\widehat\beta).
\end{aligned}
$$

Equality holds exactly when every $c_i=0$, which gives $a_i=x_i/S_{xx}$ and $\widetilde\beta=\widehat\beta$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
