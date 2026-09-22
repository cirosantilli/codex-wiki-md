<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

First derive the [survival renewal equation for a classical risk model](../../../../../survival-renewal-equation-for-a-classical-risk-model.md). Before the first claim, capital rises deterministically. The first interarrival time has [exponential distribution](../../../../../exponential-distribution.md) of rate $\lambda$, independently of the claim size. Conditioning on its time and size, and using the [Markov property](../../../../../markov-property.md) after that claim, gives

$$
\varphi(u)=\int_0^\infty\lambda e^{-\lambda t}
\int_0^{u+ct}\varphi(u+ct-x)f(x)\,dx\,dt.
$$

A claim larger than the capital available then causes immediate ruin and contributes zero. There is almost surely a first claim because $\lambda>0$.

Put $g(v)=\int_0^v\varphi(v-x)f(x)\,dx$. Changing variables $v=u+ct$ yields

$$
\varphi(u)=\frac{\lambda}{c}e^{\lambda u/c}
\int_u^\infty e^{-\lambda v/c}g(v)\,dv.
$$

Since $0\le g\le1$, this representation makes $\varphi$ locally absolutely continuous, and differentiation gives, at least almost everywhere,

$$
c\varphi'(u)=\lambda\varphi(u)-\lambda\int_0^u\varphi(u-x)f(x)\,dx.
$$

Integrate from $0$ to $u$. The integrands are nonnegative, so [Tonelli theorem](../../../../../tonelli-theorem.md) permits interchange in the double integral. In particular

$$
\int_0^u\int_0^v\varphi(v-x)f(x)\,dx\,dv
=\int_0^u\varphi(w)F(u-w)\,dw.
$$

Subtracting this from $\int_0^u\varphi(w)\,dw$, changing variables once more, and using the permitted boundary value gives

$$
\boxed{\varphi(u)=1-\frac{\lambda\mu}{c}
+\frac{\lambda}{c}\int_0^u\varphi(u-x)\bigl(1-F(x)\bigr)\,dx.}
$$

The constant is the [zero-capital survival probability](../../../../../zero-capital-survival-probability.md). Positive [relative safety loading](../../../../../relative-safety-loading.md) means $c>\lambda\mu$, so it is positive. The convolution kernel is a multiple of the [integrated tail distribution](../../../../../integrated-tail-distribution.md) density and has total mass $\lambda\mu/c<1$, making this a [defective renewal equation](../../../../../defective-renewal-equation.md).

For the individual portfolios define $\rho_i=\lambda_i\mu_i/c_i$. Under the positive-loading convention of the question, $0<\rho_i<1$. At zero capital, portfolio $i$ survives with probability $1-\rho_i$. The [independence of random variables](../../../../../independent-random-variables.md) of the entire portfolio processes makes their ultimate survival events independent. Consequently

$$
\boxed{\mathbb P(\text{all individual portfolios survive})
=\prod_{i=1}^n\left(1-\frac{\lambda_i\mu_i}{c_i}\right).}
$$

The exponential form is not needed for this zero-capital probability under positive loading; only the claim mean enters. For completeness, the company description does not separately repeat positive loading for every portfolio. If nonpositive loadings are allowed, [certain ruin with nonpositive loading and finite claim variance](../../../../../certain-ruin-with-nonpositive-loading-and-finite-claim-variance.md) instead gives

$$
\boxed{\mathbb P(\text{all individual portfolios survive})
=\prod_{i=1}^n(1-\rho_i)_+.}
$$

Here the [positive part](../../../../../positive-part-of-a-real-valued-function.md) sets a nonpositive factor to zero. To justify the additional case, observe capital at claim times: its independent increments are $c_iT-X$, with mean $c_i/\lambda_i-\mu_i$. A negative mean sends their partial sums to $-\infty$ by the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md). At zero mean, these increments have finite nonzero variance. The [central limit theorem](../../../../../central-limit-theorem.md) gives $\mathbb P(S_k<-K)\to1/2$ for each fixed $K$, so the probability of unboundedness below is at least $1/2$. That event is unchanged by altering finitely many increments and hence is a tail event; the [Kolmogorov zero-one law](../../../../../kolmogorov-s-zero-one-law.md) makes its probability one. Ruin therefore occurs almost surely also at zero loading.

For the merged claims, [Poisson superposition of insurance portfolios](../../../../../poisson-superposition-of-insurance-portfolios.md) gives total arrival rate $\lambda=\sum_i\lambda_i$. Each arrival is from portfolio $i$ with probability $\lambda_i/\lambda$, independently of other arrival labels. Thus its claim-size [mixture distribution](../../../../../mixture-distribution.md) has density

$$
\boxed{f(x)=\sum_{i=1}^n\frac{\lambda_i}{\lambda}\frac{1}{\mu_i}e^{-x/\mu_i},\qquad x>0.}
$$

The weights sum to one, so this density integrates to one. An independent transform verification uses the aggregate for one accounting period. If $M_i(r)=(1-\mu_i r)^{-1}$, then its [moment-generating function](../../../../../moment-generating-function.md) is

$$
\prod_i\exp\bigl(\lambda_i(M_i(r)-1)\bigr)
=\exp\left(\lambda\left[\sum_i\frac{\lambda_i}{\lambda}M_i(r)-1\right]\right).
$$

This is precisely a [compound Poisson distribution](../../../../../compound-poisson-distribution.md) with parameter $\lambda$ and the displayed claim-size law. The transform identity can safely be read at $r\le0$; positive arguments must be below the relevant poles.

Premium incomes and initial capitals add. Therefore the merged premium rate is $C=\sum_i c_i$, the merged initial capital is zero, and its mean claim size is

$$
\overline\mu=\sum_i\frac{\lambda_i}{\lambda}\mu_i,
\qquad \lambda\overline\mu=\sum_i\lambda_i\mu_i.
$$

Its [zero-capital survival probability](../../../../../zero-capital-survival-probability.md) is consequently

$$
\boxed{\mathbb P(\text{merged portfolio survives})
=1-\frac{\sum_i\lambda_i\mu_i}{\sum_i c_i}
=\sum_i\frac{c_i}{C}(1-\rho_i).}
$$

Under the question's positive-loading context this is a premium-weighted average of the individual survival probabilities, rather than their product. If arbitrary individual loadings are admitted, recompute the loading of the merged portfolio; its finite-variance mixture law gives the complete formula

$$
\boxed{\mathbb P(\text{merged portfolio survives})
=\left(1-\frac{\sum_i\lambda_i\mu_i}{\sum_i c_i}\right)_+.}
$$

An individually nonpositive loading does not force merged ruin when aggregate premiums still exceed aggregate expected claims. The [survival probability under risk pooling](../../../../../survival-probability-under-risk-pooling.md) is at least their product because a product of numbers in $[0,1]$ is at most each factor. Pooling allows one portfolio's surplus to cover another's deficit, so merged survival does not require every original portfolio to remain solvent separately.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
