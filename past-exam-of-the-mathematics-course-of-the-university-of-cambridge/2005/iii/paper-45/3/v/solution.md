<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Integrating the acceptance [probability](../../../../../../probability.md) over the joint-prior proposal gives

$$
\boxed{\alpha=E_g[a_k(\theta,T)]=m_k=P_{\mathrm{prior}}(S=k).}
$$

The [mean](../../../../../../expected-value.md) number of independent proposal trials per acceptance is $1/m_k$, by the [geometric distribution](../../../../../../geometric-distribution.md). To make the acceptance rate explicit for an arbitrary specified [prior](../../../../../../prior-probability.md), define the [segregating-site likelihood under the neutral coalescent](../../../../../../segregating-site-likelihood-under-the-neutral-coalescent.md) by $\ell_k(\theta)=E_T[a_k(\theta,T)]$. Then

$$
m_k=\int_0^\infty\pi(\theta)\ell_k(\theta)\,d\theta,\qquad \sum_{k\ge0}\ell_k(\theta)z^k=\prod_{i=1}^{n-1}\frac{i}{i+\theta(1-z)}.
$$

For the last identity, $W=L/2$ is the sum of independent exponential variables with rates $1,\ldots,n-1$; combine their Laplace transforms with the conditional Poisson [probability generating function](../../../../../../probability-generating-function.md). If an explicit mass is wanted, $W$ also has density $(n-1)e^{-w}(1-e^{-w})^{n-2}$: it is the maximum of $n-1$ independent unit exponential variables, whose successive spacings have exactly these exponential rates. Expanding $(1-e^{-w})^{n-2}$ and integrating the Poisson mass gives

$$
\ell_k(\theta)=(n-1)\theta^k\sum_{r=0}^{n-2}\frac{(-1)^r\binom{n-2}{r}}{(\theta+r+1)^{k+1}}.
$$

Use $\theta^0=1$ for $k=0$. The positive integral or generating-function expression may be numerically preferable to this alternating sum.

A sharper rejection envelope improves the algorithm without changing its proposal. For $k>0$, maximize the Poisson mass over $\lambda=\theta L/2$:

$$
\frac{d}{d\lambda}\log\!\left(\frac{e^{-\lambda}\lambda^k}{k!}\right)=-1+\frac{k}{\lambda}.
$$

It increases until $\lambda=k$ and decreases afterwards, so its maximum is $M_k=e^{-k}k^k/k!$. For $k=0$, the maximum is $M_0=1$. Replace the acceptance rule by $U\le a_k(\theta,T)/M_k$. This is bounded by one, and its accepted density is unchanged because the factor $1/M_k$ cancels on normalization. Thus

$$
\boxed{\alpha_{\mathrm{improved}}=\frac{m_k}{M_k},\qquad M_k=\frac{e^{-k}k^k}{k!}\ (k>0),\quad M_0=1.}
$$

For $k>0$ it is strictly more efficient, with improvement factor $1/M_k\sim\sqrt{2\pi k}$ by [Stirling's formula](../../../../../../stirling-formula.md). For $k=0$ this envelope improvement gives no increase. Evaluating the Poisson mass and using a uniform draw also avoids generating a Poisson count only to discard it. A proposal concentrated near the [posterior](../../../../../../bayesian-posterior.md) can improve efficiency further, but then its density and a valid rejection bound must be included.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
