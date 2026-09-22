<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First take $k$ to be a nonnegative integer. The [exponential tilting](../../../../../../exponential-tilting.md) constructed from the independent increments restricts to $\mathbb P_n^\lambda$ on each $\mathcal F_n$. Since its [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) is strictly positive, finite-time change of measure gives

$$
\mathbb P(\tau_k\leq n)=\mathbb E^\lambda[(M_n^\lambda)^{-1}\mathbf1_{\{\tau_k\leq n\}}].
$$

Under the tilted law, $L_n=(M_n^\lambda)^{-1}$ is a [martingale](../../../../../../martingale-split.md), because

$$
\mathbb E^\lambda[\phi(\lambda)e^{-\lambda X_{n+1}}]=\int\phi(\lambda)e^{-\lambda x}\frac{e^{\lambda x}}{\phi(\lambda)}\,\mu(dx)=1.
$$

Use the [stopped likelihood ratio under exponential tilting](../../../../../../stopped-likelihood-ratio-under-exponential-tilting.md) at this finite horizon. In detail, $\{\tau_k=j\}\in\mathcal F_j$, so

$$
\begin{aligned}
\mathbb E^\lambda[L_n\mathbf1_{\{\tau_k\leq n\}}]
&=\sum_{j=0}^n\mathbb E^\lambda[\mathbb E^\lambda(L_n\mid\mathcal F_j)\mathbf1_{\{\tau_k=j\}}]\\
&=\sum_{j=0}^n\mathbb E^\lambda[L_j\mathbf1_{\{\tau_k=j\}}]
=\mathbb E^\lambda[L_{\tau_k}\mathbf1_{\{\tau_k\leq n\}}].
\end{aligned}
$$

Here the last expression is defined only on the displayed event, so no value of $M_\infty^\lambda$ is being assumed. The [upward skip-free random walk](../../../../../../upward-skip-free-random-walk.md) has integer increments bounded above by one, which imply $S_{\tau_k}=k$ on a finite hit: the preceding value is at most $k-1$, and there is no upward overshoot. Consequently

$$
\boxed{\mathbb P(\tau_k\leq n)=e^{-\lambda k}\mathbb E^\lambda[\phi(\lambda)^{\tau_k}\mathbf1_{\{\tau_k\leq n\}}].}
$$

At $\lambda=\lambda_0$, the [mean under one-sided exponential tilting](../../../../../../mean-under-one-sided-exponential-tilting.md) is finite and positive. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $S_n/n\to\phi'(\lambda_0)>0$ under $\mathbb P^{\lambda_0}$, so every integer level is hit [almost surely](../../../../../../almost-sure-convergence.md). Since $\phi(\lambda_0)=1$, passing to $n\to\infty$ gives

$$
\boxed{\mathbb P(\tau_k<\infty)=e^{-\lambda_0k},\qquad k\in\mathbb Z_{\geq0}.}
$$

Let $H=\sup_{n\geq0}S_n$. The event $\{H\geq k\}$ is exactly the finite-hit event: an integer sequence with all its values below $k$ has supremum at most $k-1$. Also $\mathbb P(H=\infty)=\lim_k e^{-\lambda_0k}=0$. Subtraction of consecutive tail probabilities gives the [geometric maximum of an upward skip-free random walk](../../../../../../geometric-maximum-of-an-upward-skip-free-random-walk.md):

$$
\boxed{\mathbb P(H=j)=(1-e^{-\lambda_0})e^{-\lambda_0j},\qquad j=0,1,2,\ldots.}
$$

This is the [geometric distribution](../../../../../../geometric-distribution.md) counting failures before the first success, with success parameter $1-e^{-\lambda_0}$.

The PDF writes only $k\geq0$, without explicitly declaring integer levels. If it is read as allowing real $k$, then $\tau_k=\tau_{\lceil k\rceil}$ and the displayed factor must be $e^{-\lambda\lceil k\rceil}$; the hitting probability is likewise $e^{-\lambda_0\lceil k\rceil}$. For example, increments $+1$ and $-1$ with probabilities $1/3$ and $2/3$ have $\lambda_0=\log2$: hitting level $1/2$ has probability $1/2$, not $2^{-1/2}$. The integer interpretation supplies the intended formula.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
