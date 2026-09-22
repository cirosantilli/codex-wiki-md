<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

The [law of total probability](../../../../../law-of-total-probability.md) and the definition of [conditional probability](../../../../../conditional-probability.md) give [Bayes' theorem](../../../../../bayes-theorem.md):

$$
P(A_i\mid E)=\frac{P(A_i\cap E)}{P(E)}
=\frac{P(A_i)P(E\mid A_i)}{\sum_{j=1}^3P(A_j)P(E\mid A_j)}.
$$

The denominator is positive because $P(E)>0$.

For the observed cargo, set $p_A=0.05$, $p_B=0.03$, $p_C=0.01$. The [binomial likelihood](../../../../../binomial-likelihood.md) under origin $i$ is

$$
L_i=P(E\mid A_i)=\binom{10000}{200}p_i^{200}(1-p_i)^{9800}.
$$

Equal prior probabilities and [Bayes' theorem](../../../../../bayes-theorem.md) make the posterior proportional to these likelihoods. The binomial coefficient cancels in the [likelihood ratios](../../../../../likelihood-ratio.md):

$$
\begin{aligned}
\log\frac{L_A}{L_B}
&=200\log\frac53+9800\log\frac{0.95}{0.97}\approx-102.00893,\\
\log\frac{L_C}{L_B}
&=-200\log3+9800\log\frac{0.99}{0.97}\approx-19.71552.
\end{aligned}
$$

Thus $L_A/L_B\approx4.99\times10^{-45}$ and $L_C/L_B\approx2.74\times10^{-9}$, giving

$$
\boxed{P(B\mid E)=\frac1{1+L_A/L_B+L_C/L_B}
\approx0.99999999726.}
$$

Even the permitted approximation $\log(1-p)\approx-p$ gives log ratios about $-93.83$ and $-23.72$, which already show overwhelming posterior preference for B. The exact logarithms are preferable because multiplication by $9800$ magnifies the approximation error. An observed contamination fraction halfway between two hypothesized rates does not give equal [likelihoods](../../../../../likelihood-function.md): the [binomial distribution](../../../../../binomial-distribution.md) assigns asymmetric probabilities to those deviations, especially at this large sample size.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
