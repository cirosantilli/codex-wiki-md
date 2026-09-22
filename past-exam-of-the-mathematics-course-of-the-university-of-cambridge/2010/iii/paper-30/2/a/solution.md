<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A multiclass queue must specify its [service discipline](../../../../../../service-discipline.md) as well as its arrival and service rates. Here is an ordered-queue model that includes the usual class-independent exponential single-server queue. Let class-$r$ arrivals be independent [Poisson processes](../../../../../../poisson-process.md) of rates $\alpha_r$, and let a class-$r$ service requirement have the [exponential distribution](../../../../../../exponential-distribution.md) of rate $\mu_r$. A state is a finite word $x=(c_1,\ldots,c_n)$ of customer classes.

Choose service fractions $\gamma_i(n)\geq0$ with $\sum_{i=1}^n\gamma_i(n)=1$, and insertion probabilities $\delta_i(n)\geq0$ with $\sum_{i=1}^n\delta_i(n)=1$. The customer at position $i$ departs at rate $\mu_{c_i}\gamma_i(n)$; a class-$r$ arrival is inserted at position $i$ at rate $\alpha_r\delta_i(n+1)$. All rates leading to the same word are added. For class-dependent $\mu_r$, impose the [symmetric service discipline](../../../../../../symmetric-service-discipline.md) $\delta_i(n)=\gamma_i(n)$. If all $\mu_r=\mu$, arbitrary class-independent $\gamma,\delta$ are permitted, including [first come first served](../../../../../../first-come-first-served.md) with insertion at the tail and service at the head.

Put $\rho_r=\alpha_r/\mu_r$ and $\rho=\sum_r\rho_r$. For $\rho<1$, the equilibrium word law is

$$
\boxed{\pi(c_1,\ldots,c_n)=(1-\rho)\prod_{i=1}^n\rho_{c_i}.}
$$

For the [symmetric service discipline](../../../../../../symmetric-service-discipline.md), insertion and deletion satisfy [detailed balance for a continuous-time Markov chain](../../../../../../detailed-balance-for-a-continuous-time-markov-chain.md) because

$$
\pi(x)\alpha_r\gamma_i(n+1)=\pi(\operatorname{ins}_{i,r}x)\mu_r\gamma_i(n+1).
$$

For the common-service-rate case, use [time reversal of a continuous-time Markov chain](../../../../../../time-reversal-of-a-continuous-time-markov-chain.md) instead: the reversed queue inserts with probabilities $\gamma$ and serves with fractions $\delta$. A forward insertion gives a reverse deletion rate $\mu\delta_i$, and a forward deletion gives a reverse insertion rate $\alpha_r\gamma_i$. Forward and reverse total rates both equal $\sum_r\alpha_r+\mu\mathbf1_{\{n>0\}}$, proving [global balance for a continuous-time Markov chain](../../../../../../global-balance-for-a-continuous-time-markov-chain.md).

Summing the weights of all words of length $n$ gives $(1-\rho)\rho^n$, so the law is normalized. If $n_r$ counts class-$r$ customers and $n=\sum_r n_r$, the [multinomial coefficient](../../../../../../multinomial-coefficient.md) counting class orderings gives

$$
\boxed{\pi((n_r)_r)=(1-\rho)n!\prod_r\frac{\rho_r^{n_r}}{n_r!}.}
$$

For [processor sharing](../../../../../../processor-sharing.md), $\gamma_i(n)=\delta_i(n)=1/n$, the class-count vector itself is a [Markov chain](../../../../../../markov-chain.md), with arrival rate $\alpha_r$ and departure rate $\mu_r n_r/n$. Under [first come first served](../../../../../../first-come-first-served.md), the ordered word is generally necessary. Class-dependent service rates combined with [first come first served](../../../../../../first-come-first-served.md) do not in general have the displayed simple equilibrium law; the discipline assumption matters.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
