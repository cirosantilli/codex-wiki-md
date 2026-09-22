<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

There is a notation problem here. The [posterior predictive probability](../../../../../../posterior-predictive-probability.md) $p_0$ calculated above is already a fixed number conditional on $a,b,n,T$. Literally,

$$
\boxed{\mathbb P(p_0<1/2\mid\mathcal D)=\mathbf1\!\left\{(B/(B+1))^A<1/2\right\}.}
$$

No simulation is needed for that interpretation. The known exposure $T$ is also necessary, despite its omission from this part's list of inputs.

The natural uncertain quantity is instead $q(\lambda)=\mathbb P(M=0\mid\lambda)=e^{-\lambda}$. For its [posterior probability](../../../../../../posterior-probability.md) of being below one half, draw the rate from its [gamma distribution](../../../../../../gamma-distribution.md) [Bayesian posterior](../../../../../../bayesian-posterior.md) and average an indicator. Rough [BUGS](../../../../../../bugs.md) code is
```
model {
  lambda ~ dgamma(a+n, b+T)
  q <- exp(-lambda)
  belowHalf <- step(lambda-log(2))
}
```
The monitored average of `belowHalf` estimates **$\mathbb P(\lambda>\log2\mid\mathcal D)$**, equivalently $1-F_{\operatorname{Gamma}(A,B)}(\log2)$. The equality boundary has zero probability. This code samples the already updated [Bayesian posterior](../../../../../../bayesian-posterior.md); adding the count [likelihood function](../../../../../../likelihood-function.md) again would count the data twice.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
