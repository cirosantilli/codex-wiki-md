# Three Bernoulli variables through characteristic functions

↑ **Parent:** [Characteristic function of a sum of independent variables](characteristic-function-of-a-sum-of-independent-variables.md)

Let $B_1,B_2,B_3$ be [independent random variables](independent-random-variables.md), each with the [Bernoulli distribution](bernoulli-distribution.md) of parameter $1/3$, and let $S=B_1+B_2+B_3$. Multiplying their [characteristic functions](characteristic-function-split.md) and expanding by the [binomial theorem](binomial-theorem.md) gives

$$
\varphi_S(t)=\left(\frac23+\frac13e^{it}\right)^3
=\frac8{27}+\frac{12}{27}e^{it}+\frac6{27}e^{2it}+\frac1{27}e^{3it}.
$$

The coefficients are exactly the [probability mass function](probability-mass-function.md) of the [binomial distribution](binomial-distribution.md) with parameters $3,1/3$: the sum takes $0,1,2,3$ with [probabilities](probability.md) $8/27,12/27,6/27,1/27$. Direct outcome counting verifies them: an outcome with $k$ ones has [probability](probability.md) $(1/3)^k(2/3)^{3-k}$, and there are $\binom3k$ such outcomes. The coefficients sum to one, recovering $\varphi_S(0)=1$.

At $t=\pi$, $\varphi_S(\pi)=(1/3)^3=1/27$. This is also $\mathbb P(S\text{ even})-\mathbb P(S\text{ odd})=(8+6-12-1)/27$: the [complex exponential](complex-exponential-function.md) now records [parity](parity.md). The [moments](moment.md) agree by two routes: [linearity of expectation](linearity-of-expectation.md) gives $\mathbb E[S]=1$, while the [variance of a sum](variance-of-a-sum.md) of [independent random variables](independent-random-variables.md) gives $\operatorname{Var}(S)=3(2/9)=2/3$. Summing $k^2\mathbb P(S=k)$ gives the [second moment](second-moment.md) $5/3$, also recovered as $-\varphi_S''(0)$.

<a id="image-independent-products-and-the-different-limits-of-averages-and-variance-normalized-sign-sums"></a>
![](characteristic-function-independent-sums-and-scaling.png)

**[Figure 2](#image-independent-products-and-the-different-limits-of-averages-and-variance-normalized-sign-sums). Independent products and the different limits of averages and variance-normalized sign sums**. Top: exact [real parts](real-part.md) and [imaginary parts](imaginary-part.md) of $\varphi_B(t)=2/3+e^{it}/3$ and its cube, the [characteristic function](characteristic-function-split.md) of the three-variable [binomial distribution](binomial-distribution.md). Bottom: for [independent](independent-random-variables.md) symmetric signs, $\cos(t/n)^n$ approaches one under averaging, whereas $\cos(t/\sqrt n)^n$ approaches $e^{-t^2/2}$ under [variance normalization](variance-normalization.md). All curves are exact model formulas; the finite curves illustrate the two limits rather than proving a general [central limit theorem](central-limit-theorem.md).

## ↑ Ancestors (7)

1. [Characteristic function of a sum of independent variables](characteristic-function-of-a-sum-of-independent-variables.md)
2. [Characteristic function](characteristic-function-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
