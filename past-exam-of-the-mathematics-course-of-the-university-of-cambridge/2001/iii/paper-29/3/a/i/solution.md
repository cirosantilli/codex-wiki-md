<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat each release as an independent Bernoulli observation with a two-week event [probability](../../../../../../../probability.md), giving two independent [binomial distributions](../../../../../../../binomial-distribution.md). Under the specified effect, the [probabilities](../../../../../../../probability.md) are $p_0=0.0016$ and $p_1=0.0008$ with $n=15000$ in each period. The expected event counts are therefore 24 and 12. For a conventional two-sided 5% comparison of proportions, let $D=\widehat p_0-\widehat p_1$, $\delta=p_0-p_1=0.0008$ and $\bar p=(p_0+p_1)/2=0.0012$. Use

$$
s_0=\sqrt{\frac{2\bar p(1-\bar p)}n}=0.00039976,\qquad
s_1=\sqrt{\frac{p_0(1-p_0)+p_1(1-p_1)}n}=0.00039973.
$$

The approximate null rejection region is $|D|>1.96s_0$, and under the alternative $D$ is approximately $N(\delta,s_1^2)$. Thus the [power of a two-sample rare-event comparison](../../../../../../../power-of-a-two-sample-rare-event-comparison.md) is

$$
\begin{aligned}
\operatorname{Power}
&\approx1-\Phi\left(\frac{1.96s_0-\delta}{s_1}\right)
+\Phi\left(\frac{-1.96s_0-\delta}{s_1}\right)\\
&\approx0.5165.
\end{aligned}
$$

Here $\Phi$ is the [standard normal distribution function](../../../../../../../standard-normal-distribution-function.md). Hence the normal approximation gives $\boxed{\text{two-sided power approximately }52\%}$: detecting the proposed halving is far from assured.

For the small counts, a discrete calculation is also appropriate. Approximate the two counts by independent [Poisson distributions](../../../../../../../poisson-distribution.md) with means 24 and 12. Conditional on their total $K$, the pre-intervention count is $\operatorname{Binomial}(K,1/2)$ under equal rates and $\operatorname{Binomial}(K,2/3)$ under the halving alternative; $K\sim\operatorname{Poisson}(36)$ under that alternative. If $\mathcal R_k$ is the rejection set of the symmetric exact two-sided 5% binomial test, its power is

$$
\sum_{k=0}^{\infty}e^{-36}\frac{36^k}{k!}
\sum_{j\in\mathcal R_k}\binom kj(2/3)^j(1/3)^{k-j}\approx0.454.
$$

This conservative discrete test has about 45% power, lower than the normal approximation because its achieved level can be below 5%. If a decrease-only one-sided 5% test had been specified in advance, replace 1.96 by 1.645; the normal-approximation power is about 64%. The tail convention and the chosen test must accompany any quoted [statistical power](../../../../../../../statistical-power.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 29](../../../../paper-29-split.md)
5. [Iii](../../../../split.md)
6. [2001](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
