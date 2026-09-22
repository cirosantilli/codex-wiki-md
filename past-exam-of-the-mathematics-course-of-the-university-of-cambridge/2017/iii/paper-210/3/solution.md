<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $p=dP/d\nu$ and $q=dQ/d\nu$ be [Radon-Nikodym derivatives](../../../../../radon-nikodym-derivative.md). Use the following normalizations of the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md), [total variation distance](../../../../../total-variation-distance.md) and [unnormalized Hellinger distance](../../../../../unnormalized-hellinger-distance.md):

$$
\boxed{\begin{aligned}
\operatorname{KL}(P,Q)&=\int p\log(p/q)\,d\nu,\\
\operatorname{TV}(P,Q)&=\sup_{A\in\mathcal A}|P(A)-Q(A)|=\frac12\int|p-q|\,d\nu,\\
h(P,Q)^2&=\int(\sqrt p-\sqrt q)^2\,d\nu.
\end{aligned}}
$$

We use $0\log(0/q)=0$ and assign infinite [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) if $P
ot\ll Q$, where $\ll$ denotes [absolute continuity of measures](../../../../../absolute-continuity-of-measures.md). Common domination alone also suffices for the inequalities with the extended-value convention. The negative part of the logarithmic integral is integrable: on $p<q$, $p\log(q/p)\leq q-p\leq q$. Thus the extended-value integral defining the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) is well-defined. These expressions do not depend on which common dominating measure is chosen. The [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) is generally asymmetric and therefore fails a defining property of a [metric](../../../../../metric.md).

For completeness, the integral formula for [total variation distance](../../../../../total-variation-distance.md) follows by taking $A=\{p\geq q\}$: since $\int(p-q)\,d\nu=0$, the positive and negative parts of $p-q$ have the same integral, and this set attains the supremum.

Put $a=\int\sqrt{pq}\,d\nu\leq1$, by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). A second application gives

$$
\begin{aligned}
\operatorname{TV}(P,Q)
&=\frac12\int|\sqrt p-\sqrt q|(\sqrt p+\sqrt q)\,d\nu\\
&\leq\frac{h(P,Q)}2\left(\int(\sqrt p+\sqrt q)^2\,d\nu\right)^{1/2}\\
&=\frac h2\sqrt{2+2a}\leq h.
\end{aligned}
$$

The logarithmic inequality in the hint implies $\log t\leq t-1$ for $t>0$. Apply it to $t=\sqrt{q/p}$ on $\{p>0\}$:

$$
-\log(q/p)\geq2(1-\sqrt{q/p}).
$$

Multiplying by $p$ and integrating proves

$$
\operatorname{KL}(P,Q)\geq2-2\int\sqrt{pq}\,d\nu=h(P,Q)^2.
$$

If $q=0<p$ on a set of positive $P$-measure, the right side is finite but the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) is infinite, so the inequality is immediate. Thus

$$
\boxed{\operatorname{TV}(P,Q)\leq h(P,Q)\leq\sqrt{\operatorname{KL}(P,Q)}.}
$$

This [total variation–Hellinger–relative entropy inequality](../../../../../total-variation-hellinger-relative-entropy-inequality.md) requires the stated [Hellinger distance](../../../../../hellinger-distance.md) normalization for its first constant. With the alternative convention $\bar h^2=\tfrac12\int(\sqrt p-\sqrt q)^2$, the correct comparison is $\operatorname{TV}\leq\sqrt2\,\bar h$ and $\bar h\leq\sqrt{\operatorname{KL}/2}$. In particular, $P=\operatorname{Bernoulli}(0.6)$ and $Q=\operatorname{Bernoulli}(0.4)$ have $\operatorname{TV}=0.2>\bar h\approx0.1421$.

Here is a testing form of the [Le Cam two-point lemma](../../../../../le-cam-two-point-lemma.md). Suppose two parameter values $\theta_0,\theta_1$ in a [metric space](../../../../../metric-space.md) have separation $\Delta=d(\theta_0,\theta_1)>0$, and let $P_0,P_1$ be the corresponding observation laws. Every [estimator](../../../../../estimator.md) $T$ satisfies

$$
\boxed{\max_{j=0,1}P_j\{d(T,\theta_j)\geq\Delta/2\}
\geq\frac{1-\operatorname{TV}(P_0,P_1)}2.}
$$

To prove it, classify $T$ by the closer of the two parameters, breaking a tie in favour of one. Let $A=\{d(T,\theta_1)\leq d(T,\theta_0)\}$. On $A$, the [triangle inequality](../../../../../triangle-inequality.md) implies $d(T,\theta_0)\geq\Delta/2$, while on $A^c$ it implies $d(T,\theta_1)>\Delta/2$. Hence the sum of the two probabilities in the display is at least

$$
P_0(A)+P_1(A^c)=1-\{P_1(A)-P_0(A)\}\geq1-\operatorname{TV}(P_0,P_1).
$$

At least one is at least half the sum, proving the claim. It also gives a lower bound $\Delta(1-\operatorname{TV})/4$ for the maximum expected metric loss.

For [absolute-error loss](../../../../../absolute-error-loss.md), or any loss given by a [metric](../../../../../metric.md), there is a stronger expectation form. Take densities $p_0,p_1$ relative to $m=P_0+P_1$ and use the [triangle inequality](../../../../../triangle-inequality.md) under their overlap:

$$
\begin{aligned}
\mathbb E_0d(T,\theta_0)+\mathbb E_1d(T,\theta_1)
&\geq\int\min(p_0,p_1)\{d(T,\theta_0)+d(T,\theta_1)\}\,dm\\
&\geq\Delta\int\min(p_0,p_1)\,dm
=\Delta\{1-\operatorname{TV}(P_0,P_1)\}.
\end{aligned}
$$

Therefore the [Le Cam lower bound under absolute-error loss](../../../../../le-cam-lower-bound-under-absolute-error-loss.md) is

$$
\boxed{\max_{j=0,1}\mathbb E_j|T-\theta_j|
\geq\frac{|\theta_1-\theta_0|}{2}\{1-\operatorname{TV}(P_0,P_1)\}.}
$$

Both arguments are valid for randomized estimators as well, by adjoining the [independent](../../../../../independent-random-variables.md) randomization to the observation; doing so does not change [total variation distance](../../../../../total-variation-distance.md).

For the [normal distribution](../../../../../normal-distribution.md) model, assume the usual nondegenerate convention $\sigma>0$ and use the full product observation laws. Choose

$$
\mu_0=0,\qquad\mu_1=\frac{\sigma}{\sqrt{2n}}.
$$

For one observation, its Gaussian log [likelihood ratio](../../../../../likelihood-ratio.md) is

$$
\log\frac{p_0(X)}{p_1(X)}=\frac{(X-\mu_1)^2-(X-\mu_0)^2}{2\sigma^2}.
$$

Under the first law, $\mathbb E_0(X-\mu_1)^2=\sigma^2+(\mu_1-\mu_0)^2$ and $\mathbb E_0(X-\mu_0)^2=\sigma^2$. Thus the [Kullback-Leibler divergence between normal distributions](../../../../../kullback-leibler-divergence-between-normal-distributions.md) is

$$
\operatorname{KL}\!\left(N(\mu_0,\sigma^2),N(\mu_1,\sigma^2)\right)
=\frac{(\mu_1-\mu_0)^2}{2\sigma^2}.
$$

For the [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md), the joint log [likelihood ratio](../../../../../likelihood-ratio.md) is the sum of the individual ones, so the [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) of the two full [statistical samples](../../../../../statistical-sample.md) is $n(\mu_1-\mu_0)^2/(2\sigma^2)=1/4$. The comparison just proved implies $\operatorname{TV}(P_0,P_1)\leq1/2$. Applying the expectation form of the [Le Cam two-point lemma](../../../../../le-cam-two-point-lemma.md) gives

$$
\boxed{\sup_{\mu\in\mathbb R}\mathbb E_\mu|\widetilde\mu-\mu|
\geq\frac{\sigma}{4\sqrt{2n}}
=\frac{c}{\sqrt n},\qquad c=\frac{\sigma}{4\sqrt2}>0.}
$$

This is a [Gaussian location minimax lower bound under absolute-error loss](../../../../../gaussian-location-minimax-lower-bound-under-absolute-error-loss.md). The constant may depend on the fixed known $\sigma$, but neither on the [estimator](../../../../../estimator.md) nor on $n$. If a signed nonzero scale were used, the same result holds with $|\sigma|$ in place of $\sigma$. If zero noise were allowed, $X_1=\mu$ would estimate $\mu$ exactly, so a positive lower bound would be false; positive [variance](../../../../../variance-split.md) is necessary.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
