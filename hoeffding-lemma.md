# Hoeffding lemma

↑ **Parent:** [Hoeffding inequality](hoeffding-inequality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hoeffding's_lemma)

The [Hoeffding lemma](hoeffding-lemma.md) controls the entire centered [moment-generating function](moment-generating-function.md) using only an [interval](interval-mathematics.md) width. For an [essentially bounded](essentially-bounded-function.md) real [random variable](random-variable-split.md) $X$ with finite deterministic bounds $a\leq X\leq b$ [almost surely](almost-sure-convergence.md), every real $\lambda$ satisfies

$$
\boxed{\psi(\lambda):=\log\mathbb E e^{\lambda(X-\mathbb EX)}\leq\frac{\lambda^2(b-a)^2}{8}.}
$$

Equivalently, $\mathbb E e^{\lambda(X-\mathbb EX)}\leq e^{\lambda^2(b-a)^2/8}$. This single-[random variable](random-variable-split.md) statement needs no [independence](independent-random-variables.md) assumption; [independence](independent-random-variables.md) enters when applying it to the factors for a [sum](sum.md) in the [Hoeffding inequality](hoeffding-inequality.md). Both signs of $\lambda$ are allowed, and equality holds at $\lambda=0$ or when $a=b$.[§3, p. 6, lemma 5: all-real-parameter moment-generating function bound](cs229-supplemental-lecture-notes/hoeffding%E2%80%99s-inequality.md)

In the convention $\log\mathbb E e^{\lambda Y}\leq\lambda^2\sigma^2/2$ for a centered [sub-Gaussian random variable](sub-gaussian-distribution.md) $Y$, the [Hoeffding lemma](hoeffding-lemma.md) supplies $\sigma^2=(b-a)^2/4$. This upper parameter need not equal the actual [variance](variance-split.md). For a [Bernoulli random variable](bernoulli-distribution.md) $B$ of success [probability](probability.md) $p$,

$$
\log\mathbb E e^{\lambda(B-p)}=\log(1-p+pe^\lambda)-p\lambda\leq\lambda^2/8.
$$

The actual [variance](variance-split.md) is $p(1-p)$, whereas the supplied parameter is $1/4$ for every $p$. This explains part of the conservatism visible in [Hoeffding sample size for Bernoulli frequencies](hoeffding-sample-size-for-bernoulli-frequencies.md).

<a id="image-exponential-tilting-changes-the-weights-but-preserves-the-bounded-interval"></a>
![](hoeffding-bounded-interval-exponential-tilt.png)

**[Figure 7](#image-exponential-tilting-changes-the-weights-but-preserves-the-bounded-interval). Exponential tilting changes the weights but preserves the bounded interval**. The original three-point model has $X=-2,0,2$ with [probabilities](probability.md) $1/4,1/2,1/4$ and [mean](expected-value-split.md) zero. Left: tilted masses proportional to $\mathbb P(X=x)e^{\lambda x}$ for $\lambda=-1,0,1$ stay within $[-2,2]$. Right: its [cumulant-generating function](cumulant-generating-function.md) $\psi(\lambda)=2\log\cosh\lambda$ stays below the [Hoeffding lemma](hoeffding-lemma.md) bound $2\lambda^2$. Its tilted [variance](variance-split.md) is $\psi''(\lambda)=2/\cosh^2\lambda\leq2$, smaller than the general width-only ceiling four.

A short proof exposes why the constant is $1/8$. Put $Y=X-\mathbb EX$ and define [exponential tilting](exponential-tilting.md) by

$$
d\mathbb P_\lambda=e^{\lambda Y-\psi(\lambda)}d\mathbb P.
$$

The tilted [probability measure](probability-measure.md) has the same [interval](interval-mathematics.md) of possible values, and differentiating the [cumulant-generating function](cumulant-generating-function.md) gives $\psi''(\lambda)=\operatorname{Var}_{\mathbb P_\lambda}(Y)$. Boundedness justifies these [derivatives](derivative.md) for every finite $\lambda$. Under any such tilted law, [Popoviciu's inequality on variances](popoviciu-s-inequality-on-variances.md) gives $\psi''(\lambda)\leq(b-a)^2/4$: the [variance](variance-split.md) is no larger than the [expected value](expected-value-split.md) of the squared distance from the [interval](interval-mathematics.md) midpoint, itself at most $(b-a)^2/4$. Since $\psi(0)=\psi'(0)=0$, the integral form of [Taylor's theorem](taylor-s-theorem.md) yields

$$
\psi(\lambda)=\lambda^2\int_0^1(1-s)\psi''(s\lambda)\,ds\leq\lambda^2(b-a)^2/8.
$$

This expression handles either sign of $\lambda$ without changing the argument.

The constant $1/8$ cannot be reduced uniformly over all [essentially bounded](essentially-bounded-function.md) real [random variables](random-variable-split.md). Equal endpoint [probabilities](probability.md) at $a$ and $b$ give $Y=\pm(b-a)/2$, a scaled [Rademacher random variable](rademacher-distribution.md), and

$$
\lim_{\lambda\to0}\frac{\log\mathbb E e^{\lambda Y}}{\lambda^2}=\frac{\operatorname{Var}(Y)}2=\frac{(b-a)^2}{8}.
$$

Thus the sharpness is already forced near zero by the [variance](variance-split.md); the bound need not be equality at nonzero parameters for a particular [probability distribution](probability-distribution-split.md).

## ↑ Ancestors (8)

1. [Hoeffding inequality](hoeffding-inequality.md)
2. [Concentration inequality](concentration-inequality.md)
3. [Probability inequality](probability-inequality-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Concentration of Lipschitz functions on the symmetric group](concentration-of-lipschitz-functions-on-the-symmetric-group.md)
- [Doob exposure martingale](doob-exposure-martingale.md)
- [Hoeffding inequality](hoeffding-inequality.md)
- [Hoeffding lemma](hoeffding-lemma.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-33/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-37/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-208/1/a/solution.md)
- [Spectral norm bound for a centered Bernoulli adjacency matrix](spectral-norm-bound-for-a-centered-bernoulli-adjacency-matrix.md)
