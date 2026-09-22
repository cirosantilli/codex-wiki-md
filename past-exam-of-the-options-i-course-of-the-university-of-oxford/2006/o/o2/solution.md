<h1 id="o/o2/solution">Solution</h1>

↑ **Parent:** [O2](../o2.md)

Assume each sampled response is truthful, card selection is independent of the student's status, and responses follow the usual independent sampling model. In [randomized response](../../../../randomized-response.md), a yes answer occurs either for a user receiving the first question or for a nonuser receiving the complementary question. Its probability is

$$
\boxed{q=xp+(1-x)(1-p)=(1-x)+(2x-1)p}.
$$

Consequently $Y\sim\operatorname{Bin}(n,q)$, and the [likelihood](../../../../likelihood-function.md) is

$$
L(p)=\binom nY[(1-x)+(2x-1)p]^Y[x-(2x-1)p]^{n-Y},\qquad0\leq p\leq1.
$$

For $x\ne1/2$, first maximize the [binomial likelihood](../../../../binomial-likelihood.md) in the unrestricted probability $q$: its maximum occurs at $Y/n$. Inverting the affine relation gives

$$
\widetilde p=\frac{Y-n(1-x)}{n(2x-1)}.
$$

For an interior value $0<Y<n$, the same result follows from the score

$$
\ell'(p)=(2x-1)\frac{Y-nq}{q(1-q)}.
$$

The endpoint cases follow by monotonicity. This [estimator](../../../../estimator.md) has [expected value](../../../../expected-value-split.md) $p$ and [variance](../../../../variance-split.md)

$$
\boxed{\mathbb E\widetilde p=p,\qquad\operatorname{Var}(\widetilde p)=\frac{q(1-q)}{n(2x-1)^2}=\frac{p(1-p)}n+\frac{x(1-x)}{n(2x-1)^2}}.
$$

These identities follow immediately from $\mathbb EY=nq$ and $\operatorname{Var}(Y)=nq(1-q)$.

The printed claim needs a parameter-space qualification. The admissible yes probabilities lie in $[\min(x,1-x),\max(x,1-x)]$, which may exclude $Y/n$. The constrained [maximum-likelihood estimator](../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat p_{\rm ML}=\min\{1,\max\{0,\widetilde p\}\}}.
$$

The displayed untrimmed [estimator](../../../../estimator.md) is the [maximum-likelihood estimator](../../../../maximum-likelihood-estimator.md) only when it already lies in $[0,1]$. Its [unbiased estimator](../../../../unbiased-estimator.md) property does not carry over to the clipped [estimator](../../../../estimator.md) in general. For example, if $n=1$, $x=3/4$ and $p=0$, the clipped estimate equals 1 exactly when the answer is yes, so its expectation is $1/4$, not zero. At $x=1/2$, $q=1/2$ for every $p$: the parameter is unidentifiable and the printed quotient is undefined. Thus the unbiased formula requires $x\ne1/2$, and the constrained [likelihood](../../../../likelihood-function.md) assertion requires the stated clipping.

## ↑ Ancestors (12)

1. [O2](../o2.md)
2. [O](../../o.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
