<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $t^*>t_b>t_a$, the three possible complete event orders are $t_a<t^*<t_c<t_d$, $t_a<t_c<t^*<t_d$, and $t_a<t_c<t_d<t^*$. Write $K=\phi_a/(\phi_a+\phi_b+\phi_c+\phi_d)$ and $V=\phi_b+\phi_c+\phi_d$. Their [partial likelihoods](../../../../../../partial-likelihood.md), with the final singleton factor omitted, are respectively

$$
L_1=K\frac{\phi_b}{V}\frac{\phi_c}{\phi_c+\phi_d},\qquad L_2=K\frac{\phi_c}{V}\frac{\phi_b}{\phi_b+\phi_d},\qquad L_3=K\frac{\phi_c}{V}\frac{\phi_d}{\phi_b+\phi_d}.
$$

Adding first $L_2$ and $L_3$ gives $K\phi_c/V$, and therefore

$$
L_1+L_2+L_3=K\frac{\phi_c}{V}\left(\frac{\phi_b}{\phi_c+\phi_d}+1\right)=K\frac{\phi_c}{\phi_c+\phi_d}.
$$

Thus

$$
\boxed{L_1+L_2+L_3=L_{a,b,c,d}.}
$$

This is [Cox rank-likelihood deletion consistency](../../../../../../cox-rank-likelihood-deletion-consistency.md): summing out the unobserved position of $b$ leaves the relative order information in the observed events. It is an algebraic marginalization of complete-order [probabilities](../../../../../../probability.md) under time-constant [hazard multipliers](../../../../../../hazard-multiplier.md). It does not include the [probability density function](../../../../../../probability-density-function.md) of the actual censoring time, establish the distribution of $t^*$ given all observed times, or justify informative censoring. Ignoring the censoring mechanism in the survival analysis still requires [independent censoring](../../../../../../independent-censoring.md) given the modeled [covariates](../../../../../../covariate.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
