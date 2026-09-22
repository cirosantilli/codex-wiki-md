<h1 id="o/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume [independent](../../../../independent-random-variables.md) survival times and positive rate $\lambda$. With $S=\sum_it_i$, the [likelihood](../../../../likelihood-function.md) is $L(\lambda)=\lambda^n e^{-\lambda S}$ on the observed nonnegative data. The score and negative expected second [derivative](../../../../derivative.md) are $n/\lambda-S$ and $n/\lambda^2$. For $S>0$, which holds almost surely under the model,

$$
\boxed{\widehat\lambda=\frac nS,\qquad I_{\mathrm{full}}(\lambda)=\frac n{\lambda^2}.}
$$

The usual [independent](../../../../independent-random-variables.md)-sample [likelihood](../../../../likelihood-function.md) asymptotics give $\sqrt n(\widehat\lambda-\lambda)\Rightarrow N(0,\lambda^2)$. Thus an approximate Wald [interval](../../../../interval-mathematics.md) is

$$
\boxed{\widehat\lambda\pm z_{1-\alpha/2}\frac{\widehat\lambda}{\sqrt n}.}
$$

For a positive [interval](../../../../interval-mathematics.md) with the same first-order justification, apply the [delta method](../../../../delta-method.md) to $\log\widehat\lambda$, obtaining endpoints $\widehat\lambda\exp(\pm z_{1-\alpha/2}/\sqrt n)$.

A single individual survives until $T$ with probability $s=e^{-\lambda T}$. Thus $N_T\sim\operatorname{Bin}(n,s)$ and the new [likelihood](../../../../likelihood-function.md) is $\binom n{n_T}e^{-\lambda Tn_T}(1-e^{-\lambda T})^{n-n_T}$. For $0<n_T<n$, its [maximum](../../../../maximum-of-a-subset-of-a-total-order.md) occurs at $s=n_T/n$, giving

$$
\boxed{\widetilde\lambda=-\frac1T\log\frac{n_T}n.}
$$

If $n_T=0$, the supremum occurs as $\lambda\to\infty$ and there is no finite [maximum](../../../../maximum-of-a-subset-of-a-total-order.md). If $n_T=n$, it occurs at the boundary $\lambda=0$ of the extended parameter space, or is only a supremum when the rate is required to be strictly positive.

A binomial experiment has information $n/[s(1-s)]$ for $s$. Since $ds/d\lambda=-Ts$, parameter transformation gives

$$
\boxed{I_T(\lambda)=\frac{nT^2s}{1-s}=\frac{nT^2}{e^{\lambda T}-1}.}
$$

As quantified by [Fisher information in an exponential survival snapshot](../../../../fisher-information-in-an-exponential-survival-snapshot.md), the ratio of this information to the [complete](../../../../completeness.md)-data information is $z^2/(e^z-1)$ with $z=\lambda T>0$, strictly less than one by the supplied inequality. Hence every fixed survival snapshot loses information. Under regular large-sample conditions its efficient rate estimator has larger asymptotic [variance](../../../../variance-split.md), and correspondingly wider uncertainty [intervals](../../../../interval-mathematics.md), than the estimator based on all individual survival times. This comparison concerns information and asymptotic uncertainty, not a claim that every realized [interval](../../../../interval-mathematics.md) in one experiment is wider.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [O](../../o.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
