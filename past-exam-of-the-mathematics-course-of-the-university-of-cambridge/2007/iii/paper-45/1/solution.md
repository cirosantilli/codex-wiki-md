<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Condition on the [claim count distribution](../../../../../claim-count-distribution.md). If $\mu=\mathbb EX_1$ and $v=\operatorname{Var}(X_1)$, then independence of the count and the [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) gives

$$
\mathbb E[S\mid N]=N\mu,\qquad\operatorname{Var}(S\mid N)=Nv.
$$

The empty sum is zero. The [law of total expectation](../../../../../law-of-total-expectation.md) and [law of total variance](../../../../../law-of-total-variance.md) therefore prove the [random sum of independent claims](../../../../../random-sum-of-independent-claims.md) formulas

$$
\boxed{\mathbb ES=\mathbb EN\,\mathbb EX_1,\qquad
\operatorname{Var}(S)=\mathbb EN\operatorname{Var}(X_1)+\operatorname{Var}(N)(\mathbb EX_1)^2.}
$$

For the variance calculation assume the count and severity have finite second moments; the expectation identity needs the corresponding integrability. Nonnegative claims also permit the expectation identity with extended nonnegative values.

Represent each policy payment as $S_i=B_iY_i$, where $B_i$ is a [Bernoulli random variable](../../../../../bernoulli-distribution.md) of parameter $q_i$, independent of its severity. Equivalently, $Y_i$ specifies the payment distribution conditional on a claim. Then

$$
\mathbb ES_i=q_i\mu_i,\qquad
\mathbb ES_i^2=q_i(\sigma_i^2+\mu_i^2),\qquad
\operatorname{Var}(S_i)=q_i\sigma_i^2+q_i(1-q_i)\mu_i^2.
$$

Independence of the policies makes their [variances](../../../../../variance-split.md) add. Put

$$
Q=\sum_iq_i,\qquad M=\sum_iq_i\mu_i,\qquad
A=\sum_iq_i(\sigma_i^2+\mu_i^2),\qquad C=\sum_iq_i^2\mu_i^2.
$$

The [heterogeneous individual claims model](../../../../../heterogeneous-individual-claims-model.md) consequently has

$$
\boxed{\mathbb ET=M,\qquad\operatorname{Var}(T)=A-C
=\sum_i\bigl[q_i\sigma_i^2+q_i(1-q_i)\mu_i^2\bigr].}
$$

For the Poisson approximation, define the severity [mixture distribution](../../../../../mixture-distribution.md)

$$
F=\sum_i\frac{q_i}{Q}F_i.
$$

Let $\varphi_i(t)=\mathbb E[e^{itY_i}]$ be the individual [characteristic functions](../../../../../characteristic-function.md). Conditioning on each Poisson count and then multiplying transforms of the independent policy payments gives

$$
\begin{aligned}
\mathbb E[e^{it\widetilde T}]
&=\prod_i\exp\{q_i(\varphi_i(t)-1)\}\\
&=\exp\left\{Q\left[\sum_i\frac{q_i}{Q}\varphi_i(t)-1\right]\right\}.
\end{aligned}
$$

This is [Poisson superposition of insurance portfolios](../../../../../poisson-superposition-of-insurance-portfolios.md). By the [uniqueness theorem for characteristic functions](../../../../../uniqueness-theorem-for-characteristic-functions.md),

$$
\boxed{\widetilde T\ \overset d=\ \sum_{j=1}^{K}Z_j,\qquad
K\sim\operatorname{Poisson}(Q),\quad Z_j\overset{\mathrm{iid}}\sim F,}
$$

with count and severities independent. Its [compound Poisson distribution](../../../../../compound-poisson-distribution.md) has distribution function

$$
\mathbb P(\widetilde T\leq x)=e^{-Q}\sum_{k=0}^{\infty}\frac{Q^k}{k!}F^{*k}(x),
$$

where $F^{*k}$ is the [convolution](../../../../../convolution.md) distribution of $k$ independent severities and $F^{*0}$ is the distribution concentrated at zero. Characteristic functions avoid assuming that severity moment-generating functions exist. Since $\mathbb EZ=M/Q$ and $\mathbb EZ^2=A/Q$, the random-sum formulas give

$$
\boxed{\mathbb E\widetilde T=M,\qquad\operatorname{Var}(\widetilde T)=A.}
$$

Use $T_{\mathrm B}$ to distinguish the second, compound-binomial approximation from the Poisson one. It has $K_{\mathrm B}\sim\operatorname{Bin}(n,p)$ with $p=Q/n$ and the same severity law $F$. Thus $\mathbb EK_{\mathrm B}=Q$ and $\operatorname{Var}(K_{\mathrm B})=Q(1-p)$. Applying the [random sum of independent claims](../../../../../random-sum-of-independent-claims.md) identities again gives

$$
\begin{aligned}
\operatorname{Var}(T_{\mathrm B})
&=Q\left[\frac AQ-\left(\frac MQ\right)^2\right]
+Q(1-p)\left(\frac MQ\right)^2\\
&=A-\frac{M^2}{n}.
\end{aligned}
$$

Hence

$$
\boxed{\mathbb ET_{\mathrm B}=M,\qquad\operatorname{Var}(T_{\mathrm B})=A-M^2/n.}
$$

Both approximations match the exact [expected value](../../../../../expected-value.md). The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $M^2\leq nC$, proving the [variance comparison for compound portfolio approximations](../../../../../variance-comparison-for-compound-portfolio-approximations.md):

$$
\boxed{\operatorname{Var}(T)\leq\operatorname{Var}(T_{\mathrm B})\leq\operatorname{Var}(\widetilde T).}
$$

The excess variances are respectively $C-M^2/n$ and $C$. The compound-binomial model is therefore closer in variance; equality with the exact variance occurs when all $q_i\mu_i$ are equal. This variance comparison is not a general ordering of approximation errors or tail probabilities.

The Poisson replacement is useful when all claim probabilities are small: it replaces the individual restriction of at most one claim by an unrestricted Poisson count, and the variance error is of second order in those probabilities. The compound-binomial replacement retains a count bounded by $n$, but pools both frequencies and severity laws and can lose policy-specific information. If all $q_i$ and all $F_i$ agree, it is exactly the original portfolio law. In a heterogeneous portfolio, agreement of means, or even variances, does not make either approximate law exact. Neither approximation is guaranteed accurate merely by having many policies.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
