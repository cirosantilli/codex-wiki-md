<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [kernel for density estimation](../../../../../kernel-for-density-estimation.md) $K$ with integral one and a [smoothing bandwidth](../../../../../smoothing-bandwidth.md) $h>0$, the univariate [kernel density estimator](../../../../../kernel-density-estimation.md) is

$$
\boxed{K_h(u)=\frac1hK(u/h),\qquad
\widehat f_h(x)=\frac1n\sum_{i=1}^nK_h(x-X_i).}
$$

Its [expected value](../../../../../expected-value.md) is

$$
\mathbb E\widehat f_h(x)
=\frac1n\sum_{i=1}^n\int_{\mathbb R}K_h(x-y)f(y)\,dy
=\int_{\mathbb R}K_h(x-y)f(y)\,dy
=(K_h*f)(x).
$$

This is the [convolution](../../../../../convolution.md) identity. It holds wherever the integral is defined, in particular everywhere for the bounded kernel used below. For a nonnegative [kernel for density estimation](../../../../../kernel-for-density-estimation.md), [Tonelli theorem](../../../../../tonelli-theorem.md) also gives the identity as an extended nonnegative integral. A signed [kernel for density estimation](../../../../../kernel-for-density-estimation.md) instead requires absolute integrability for this interchange.

For the centred unit-width [uniform kernel](../../../../../uniform-smoothing-kernel.md), substitute $u=(x-y)/h$:

$$
\mathbb E\widehat f_h(x)=\int_{-1/2}^{1/2}f(x-hu)\,du.
$$

Put $M=\sup_z|f''(z)|$. The [Taylor theorem with Lagrange remainder](../../../../../taylor-theorem-with-lagrange-remainder.md) gives

$$
f(x-hu)=f(x)-hu f'(x)+R(x,u),\qquad
|R(x,u)|\leq\frac{Mh^2u^2}{2}.
$$

The [odd function](../../../../../odd-function.md) term integrates to zero, while $\int_{-1/2}^{1/2}u^2\,du=1/12$. Hence the [bias of a kernel density estimator](../../../../../bias-of-a-kernel-density-estimator.md) obeys

$$
\boxed{\left|\mathbb E\widehat f_h(x)-f(x)\right|\leq\frac{Mh^2}{24}.}
$$

This is a [second-order pointwise bias bound for kernel density estimation](../../../../../second-order-pointwise-bias-bound-for-kernel-density-estimation.md). Existence and boundedness of the [second derivative](../../../../../second-derivative.md) suffice for the stated remainder; [continuity](../../../../../continuous-function.md) of that [derivative](../../../../../derivative.md) is not an extra assumption.

For concentration, write

$$
B_i=\mathbb1_{\{|X_i-x|\leq h/2\}},\qquad
p=\mathbb P(|X_1-x|\leq h/2).
$$

The $B_i$ are [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with a [Bernoulli distribution](../../../../../bernoulli-distribution.md), and $\widehat f_h(x)=(nh)^{-1}\sum_iB_i$. The required concentration bound follows from the [Hoeffding lemma](../../../../../hoeffding-lemma.md). We prove its Bernoulli case directly. With

$$
\psi(s)=\log\mathbb E e^{s(B_1-p)},
$$

we have $\psi(0)=\psi'(0)=0$ and $\psi''(s)=p_s(1-p_s)\leq1/4$, where $p_s=pe^s/(1-p+pe^s)$ is the exponentially tilted success [probability](../../../../../probability.md). Therefore $\psi(s)\leq s^2/8$ for every real $s$. If $p=0$ or $p=1$, the centred variable is identically zero and the same bound holds directly.

[Independence](../../../../../independent-random-variables.md) and the exponential form of the [Markov inequality](../../../../../markov-inequality.md) now give, for $s>0$,

$$
\mathbb P\!\left(\sum_i(B_i-p)\geq nht\right)
\leq\exp\!\left(-snht+\frac{ns^2}{8}\right).
$$

Choose $s=4ht$. Applying the same argument to the lower tail and adding the probabilities proves the [Hoeffding inequality](../../../../../hoeffding-inequality.md)

$$
\boxed{\mathbb P\!\left(\left|\widehat f_h(x)-\mathbb E\widehat f_h(x)\right|\geq t\right)
\leq2e^{-2nh^2t^2}.}
$$

To obtain the requested [variance](../../../../../variance-split.md) constant, use the additional bound that a [probability](../../../../../probability.md) is at most one. Set $Z=\widehat f_h(x)-\mathbb E\widehat f_h(x)$ and $a=2nh^2$. The [tail integral formula for moments](../../../../../tail-integral-formula-for-moments.md), justified by [Tonelli theorem](../../../../../tonelli-theorem.md), yields

$$
\begin{aligned}
\operatorname{Var}(\widehat f_h(x))
&=\mathbb E Z^2
=\int_0^\infty\mathbb P(Z^2>u)\,du\\
&\leq\int_0^\infty\min\{1,2e^{-au}\}\,du\\
&=\frac{\log2}{a}+\int_{\log2/a}^{\infty}2e^{-au}\,du
=\frac{1+\log2}{a}.
\end{aligned}
$$

Thus

$$
\boxed{\operatorname{Var}(\widehat f_h(x))\leq\frac{1+\log2}{2nh^2}.}
$$

The clipping at one is essential for this integration argument to give that constant. It is an instance of a [second moment bound from a clipped Gaussian tail](../../../../../second-moment-bound-from-a-clipped-gaussian-tail.md). The exact [Bernoulli distribution](../../../../../bernoulli-distribution.md) calculation also gives $\operatorname{Var}(\widehat f_h(x))=p(1-p)/(nh^2)\leq1/(4nh^2)$, an even stronger bound.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
