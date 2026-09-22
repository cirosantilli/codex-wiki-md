<h1 id="o/o4/solution">Solution</h1>

↑ **Parent:** [O4](../o4.md)

For $S=\sum_i t_i$, the [likelihood](../../../../likelihood-function.md) is $L(\lambda)=\lambda^ne^{-\lambda S}$, and its log derivative is $n/\lambda-S$. Thus, almost surely,

$$
\widehat\lambda=n/S,\qquad I_{\rm full}(\lambda)=n/\lambda^2.
$$

The large-sample distribution is that of the estimator, rather than of the fixed parameter: $\sqrt n(\widehat\lambda-\lambda)\xrightarrow d N(0,\lambda^2)$. A [Wald confidence interval](../../../../wald-confidence-interval.md) is consequently

$$
\boxed{\widehat\lambda\ \pm\ z_{1-\alpha/2}\widehat\lambda/\sqrt n},
$$

intersected with the positive parameter space if necessary. The unadorned parameter in the source's distribution request is interpreted as this estimator.

A single aphid survives to $T$ with probability $r=e^{-\lambda T}$, independently of the others. Hence $N_T\sim\operatorname{Bin}(n,r)$, and

$$
L_T(\lambda)=\binom n{n_T}e^{-\lambda Tn_T}(1-e^{-\lambda T})^{n-n_T},\qquad
\widetilde\lambda=-\frac1T\log(n_T/n)
$$

for $0<n_T<n$. If $n_T=n$, the optimum is at the boundary $\lambda=0$; if $n_T=0$, the [likelihood](../../../../likelihood-function.md) increases to its supremum as $\lambda\to\infty$, so there is no finite maximum [likelihood](../../../../likelihood-function.md) estimate. [Fisher information](../../../../fisher-information-matrix.md) transforms from the binomial probability parameter as

$$
I_T(\lambda)=\frac{n(r'(\lambda))^2}{r(1-r)}=\frac{nT^2}{e^{\lambda T}-1}.
$$

The given strict inequality shows

$$
\boxed{\frac{I_T(\lambda)}{I_{\rm full}(\lambda)}=\frac{(\lambda T)^2}{e^{\lambda T}-1}<1}.
$$

Thresholding discards information about how long each survival time is. The second experiment therefore has a larger information bound on [variance](../../../../variance-split.md) and larger asymptotic uncertainty for an efficient estimator. This is an expected-information comparison, rather than a claim that every realised finite-sample [confidence interval](../../../../confidence-interval.md) must be wider.

## ↑ Ancestors (12)

1. [O4](../o4.md)
2. [O](../../o.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
