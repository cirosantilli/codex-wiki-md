<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

A [critical region](../../../../../rejection-region.md) $C$ is the set of sample outcomes on which a test rejects its [null hypothesis](../../../../../null-hypothesis.md). Its [power function](../../../../../power-function-of-a-statistical-test.md) is $\beta(\theta)=\mathbb P_\theta(X\in C)$; its [size of a statistical test](../../../../../size-of-a-statistical-test.md) is $\sup_{\theta\in\Theta_0}\beta(\theta)$. Randomized tests replace the indicator of $C$ by a rejection [probability](../../../../../probability.md) $\phi(X)\in[0,1]$.

The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) states that for two simple hypotheses with densities $p_0,p_1$, the test $\phi^*$ that is one where $p_1>kp_0$, zero where $p_1<kp_0$, and randomized on equality to have null rejection [probability](../../../../../probability.md) $\alpha$, maximizes power among tests of size at most $\alpha$. Here $k\ge0$. To prove it, let $\phi$ be any competing test. Pointwise, $(\phi^*-\phi)(p_1-kp_0)\ge0$, since both factors have the same sign off the equality set. Integrating gives

$$
\mathbb E_1\phi^*-\mathbb E_1\phi\ge k(\mathbb E_0\phi^*-\mathbb E_0\phi)\ge0.
$$

This proves the lemma, including equality-set randomization and points where $p_0=0$.

Take the exponential parameter to be its rate: $p_\lambda(x)=\lambda e^{-\lambda x}$ for $x\ge0$. For $T=\sum_iX_i$, the joint [likelihood ratio](../../../../../likelihood-ratio.md) is $(\lambda_1/\lambda_0)^n e^{-(\lambda_1-\lambda_0)T}$, decreasing in $T$. Hence for $0<\alpha<1$ the most powerful test is

$$
\boxed{\text{reject when }T\le c_\alpha,\qquad \mathbb P_{\lambda_0}(T\le c_\alpha)=\alpha.}
$$

There is no boundary randomization because $T$ has a continuous [gamma distribution](../../../../../gamma-distribution.md). Its density follows by repeated convolution: $p_T(t)=\lambda^nt^{n-1}e^{-\lambda t}/(n-1)!$. Integrating by parts gives the [exponential-rate likelihood-ratio test](../../../../../exponential-rate-likelihood-ratio-test.md) power

$$
\boxed{\beta(\lambda)=1-e^{-\lambda c_\alpha}\sum_{j=0}^{n-1}\frac{(\lambda c_\alpha)^j}{j!}.}
$$

The threshold is the unique positive solution of this formula at $\lambda=\lambda_0$ with value $\alpha$. Differentiating the finite sum yields

$$
\beta'(\lambda)=c_\alpha e^{-\lambda c_\alpha}\frac{(\lambda c_\alpha)^{n-1}}{(n-1)!}>0.
$$

Thus the [power function](../../../../../power-function-of-a-statistical-test.md) is strictly increasing, and its supremum over $0<\lambda\le\lambda_0$ is $\beta(\lambda_0)=\alpha$. Therefore **the same test has size $\alpha$ for the composite null $\lambda\le\lambda_0$**. Since the threshold does not depend on the particular larger rate, it is also uniformly most powerful against all $\lambda>\lambda_0$. The endpoint sizes zero and one have their trivial constant tests.

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
