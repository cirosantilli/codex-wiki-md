<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For [excess of loss reinsurance](../../../../../excess-of-loss-reinsurance.md) with retention $M$, the direct insurer caps its payment at $M$ and the reinsurer pays the excess. Thus

$$
\boxed{Y_i=\min(X_i,M),\qquad Z_i=(X_i-M)_+.}
$$

Let $I_i=\mathbf1_{\{X_i>M\}}$ and $\alpha=\mathbb P(X_i>M)=1-F_{X_1}(M)\in(0,1)$. These are independent [Bernoulli random variables](../../../../../bernoulli-distribution.md), independent of $N$. Since $N_R=\sum_{i=1}^NI_i$, its conditional law given $N=n$ is a [binomial distribution](../../../../../binomial-distribution.md). Conditioning on $N$ therefore gives the [Bernoulli thinning](../../../../../bernoulli-thinning.md) identity

$$
\mathbb E[z^{N_R}\mid N]=(1-\alpha+\alpha z)^N,\qquad\boxed{G_{N_R}(z)=G_N(1-\alpha+\alpha z).}
$$

Here the [probability generating function](../../../../../probability-generating-function.md) may be evaluated on $0\le z\le1$, and the identity extends wherever the transforms converge.

The positive reinsurer marks have the conditional law $W\overset d=X_1-M\mid X_1>M$. Hence

$$
\boxed{F_W(w)=\begin{cases}0,&w<0,\\\dfrac{F_{X_1}(M+w)-F_{X_1}(M)}{1-F_{X_1}(M)},&w\ge0,\end{cases}\qquad f_W(w)=\frac{f_{X_1}(M+w)}{1-F_{X_1}(M)}\quad(w>0).}
$$

The independent-mark representation is justified as follows. Conditional on any fixed count and pattern of exceedance indicators, the positive excesses are independent with this same conditional law; that law depends neither on the number of exceedances nor on their locations. Averaging over the indicator pattern thus leaves the positive mark sequence independent of $N_R$. We may extend it by additional independent copies if needed, giving $S_R=\sum_{j=1}^{N_R}W_j$ with the stated independence.

Now write $q=1-p$. For [exponential distribution](../../../../../exponential-distribution.md) claim sizes of mean $\mu$,

$$
\alpha=e^{-M/\mu},\qquad\mathbb P(W>w)=\frac{e^{-(M+w)/\mu}}{e^{-M/\mu}}=e^{-w/\mu}.
$$

Thus **$W$ is exponential with the original mean $\mu$**, by [memorylessness of the exponential distribution](../../../../../memorylessness-of-the-exponential-distribution.md). The original zero-based [geometric distribution](../../../../../geometric-distribution.md) count has $G_N(z)=p/(1-qz)$. Consequently

$$
G_{N_R}(z)=\frac{p}{p+q\alpha-q\alpha z}=\frac{p_R}{1-q_Rz},\qquad p_R=\frac{p}{p+q\alpha},\quad q_R=\frac{q\alpha}{p+q\alpha}.
$$

This is the [geometric count under Bernoulli thinning](../../../../../geometric-count-under-bernoulli-thinning.md), with

$$
\boxed{\mathbb P(N_R=k)=p_Rq_R^k\quad(k=0,1,\ldots).}
$$

Finally use the [Laplace transform of a nonnegative random variable](../../../../../laplace-transform-of-a-nonnegative-random-variable.md), keeping the mass at zero. For $t\ge0$,

$$
\mathbb E e^{-tS_R}=G_{N_R}\!\left(\frac1{1+\mu t}\right)=\frac{p_R(1+\mu t)}{p_R+\mu t}=p_R+q_R\frac{p_R}{p_R+\mu t}.
$$

The last expression is the transform of a [mixture distribution](../../../../../mixture-distribution.md): mass $p_R$ at zero and, with probability $q_R$, an [exponential distribution](../../../../../exponential-distribution.md) of rate $p_R/\mu$. Uniqueness of the [Laplace transform](../../../../../laplace-transform.md) identifies this [zero-based geometric sum of exponential variables](../../../../../zero-based-geometric-sum-of-exponential-variables.md):

$$
\boxed{\mathcal L(S_R)=p_R\delta_0+q_R\operatorname{Exp}(p_R/\mu).}
$$

Equivalently, $\mathbb P(S_R=0)=p_R$ and its positive density is $q_R(p_R/\mu)e^{-p_Rs/\mu}$. Therefore **the requested exceedance probability** is

$$
\boxed{\mathbb P(S_R>s)=\frac{(1-p)e^{-M/\mu}}{p+(1-p)e^{-M/\mu}}\exp\!\left(-\frac{p\,s}{\mu[p+(1-p)e^{-M/\mu}]}\right),\qquad s>0.}
$$

The prefactor is essential: the aggregate is zero whenever no claim crosses the retention.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
