<h1 id="o/o5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $S=\sum_iX_i$. [Independence](../../../../../independent-random-variables.md) and the exponential sampling model give the [gamma distribution](../../../../../gamma-distribution.md) with density

$$
f_S(s)=\frac{\lambda^n}{\Gamma(n)}s^{n-1}e^{-\lambda s},\qquad s>0.
$$

For $n>k$, substitution $u=\lambda s$ yields

$$
\mathbb ES^{-k}=\lambda^k\frac{\Gamma(n-k)}{\Gamma(n)}.
$$

At $k=1$, $n\geq2$, this gives $\mathbb E(\bar X^{-1})=n\lambda/(n-1)$. Therefore

$$
\boxed{\widehat\lambda=\frac{n-1}{S}=\frac{n-1}{n\bar X}}
$$

is an [unbiased estimator](../../../../../unbiased-estimator.md) of the rate. For $n>2$, the same formula with $k=2$ gives

$$
\mathbb E\widehat\lambda^2=\lambda^2\frac{n-1}{n-2},\qquad
\boxed{\operatorname{Var}(\widehat\lambda)=\frac{\lambda^2}{n-2}}.
$$

For the source-allowed value $n=2$, the first moment is still finite, but the second moment contains an integral proportional to $\int_0^1s^{-1}e^{-\lambda s}ds$ and diverges. Hence **the [estimator](../../../../../estimator.md) has infinite [variance](../../../../../variance-split.md) when $n=2$**; the finite formula applies only to $n>2$.

The sample score is $n/\lambda-S$, and its [Fisher information](../../../../../fisher-information-matrix.md) is $I_n(\lambda)=n/\lambda^2$. The [Cramér-Rao lower bound](../../../../../cramer-rao-bound.md) for unbiased rate estimation is thus $\lambda^2/n$. For every $n>2$, the actual [variance](../../../../../variance-split.md) is strictly larger by the factor $n/(n-2)$. The ratio approaches one as $n$ grows, but equality is not attained at finite $n$. At $n=2$ the finite-[variance](../../../../../variance-split.md) form of the bound is inapplicable to this [estimator](../../../../../estimator.md); its infinite [variance](../../../../../variance-split.md) provides no efficiency equality.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
