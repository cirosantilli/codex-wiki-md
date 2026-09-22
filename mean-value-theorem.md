# Mean value theorem

↑ **Parent:** [Calculus](calculus-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean_value_theorem)

The [mean value theorem](mean-value-theorem.md) says that an average rate of change is attained as an instantaneous rate somewhere between the endpoints. Let $a<b$ and let the [real-valued function](real-valued-function.md) $f:[a,b]\to\mathbb R$ be [continuous](continuous-function.md) on the [closed interval](closed-real-interval.md) $[a,b]$ and [differentiable](differentiable-function.md) on the [open interval](open-interval.md) $(a,b)$. Then there exists $c\in(a,b)$ such that

$$
f'(c)=\frac{f(b)-f(a)}{b-a}.
$$

The right-hand side is the [slope](slope.md) of the [secant line](secant-line.md) joining $(a,f(a))$ to $(b,f(b))$; the left-hand side is the [slope](slope.md) of the [tangent line](tangent-line.md) at $(c,f(c))$. The [derivative](derivative.md) need not be [continuous](continuous-function.md), and the [function](function-split.md) need not be [differentiable](differentiable-function.md) at the endpoints. [OpenStax, Calculus Volume 1, Section 4.4: mean value theorem](https://openstax.org/books/calculus-volume-1/pages/4-4-the-mean-value-theorem)

For the [polynomial](polynomial-split.md) $f(x)=x^2$ on $[1,3]$, the [secant line](secant-line.md) has [slope](slope.md) $(9-1)/(3-1)=4$. Since the [derivative](derivative.md) is $f'(x)=2x$, the required interior point is $c=2$. The [tangent line](tangent-line.md) there is $y=4+4(x-2)=4x-4$, whereas the [secant line](secant-line.md) is $y=1+4(x-1)=4x-3$. Their equal [slopes](slope.md) make them parallel, but they are distinct [straight lines](straight-line.md): the theorem equates rates, not heights.

<a id="image-the-secant-line-and-interior-tangent-line-to-x-2-have-equal-slopes-but-different-heights"></a>
![](mean-value-theorem-secant-and-tangent.png)

**[Figure 14](#image-the-secant-line-and-interior-tangent-line-to-x-2-have-equal-slopes-but-different-heights). The secant line and interior tangent line to $x^2$ have equal slopes but different heights**.

The practical strength is that the unknown point $c$ can disappear from an estimate. Under the same hypotheses, if the [derivative](derivative.md) satisfies $|f'(x)|\leq M$ throughout $(a,b)$, where $M\geq0$, then

$$
|f(b)-f(a)|=|f'(c)|\,|b-a|\leq M|b-a|.
$$

Applying this to every subinterval proves [Lipschitz continuity](lipschitz-continuity.md) with [Lipschitz bound](lipschitz-bound.md) $M$. For example, $f(x)=x^2$ on $[1,3]$ has $|f'(x)|\leq6$, so an input change of size at most $\delta$ changes its output by at most $6\delta$, as long as both inputs lie in that [interval](interval-mathematics.md). A local [derivative](derivative.md) bound therefore controls finite changes without computing an [integral](integral-split.md). The sign of the [derivative](derivative.md) similarly gives the [derivative criterion for monotonicity](derivative-criterion-for-monotonicity.md).

Taking $M=0$ shows that a [function](function-split.md) with zero [derivative](derivative.md) throughout a [real interval](interval-mathematics.md) is a [constant function](constant-function.md), provided it is [continuous](continuous-function.md) at any included endpoints. The [interval](interval-mathematics.md) condition is essential: on the [domain of a function](domain-of-a-function.md) $(-2,-1)\cup(1,2)$, the [function](function-split.md) equal to zero on the left [interval](interval-mathematics.md) and one on the right [interval](interval-mathematics.md) has zero [derivative](derivative.md) everywhere. It is a [locally constant function](locally-constant-function.md), yet not a [constant function](constant-function.md) on the whole [domain of a function](domain-of-a-function.md). The [mean value theorem](mean-value-theorem.md) cannot cross the gap.

A concise proof subtracts the [secant line](secant-line.md): set $m=(f(b)-f(a))/(b-a)$ and $h(x)=f(x)-f(a)-m(x-a)$. Then $h(a)=h(b)=0$, and [Rolle's theorem](rolle-theorem.md) gives an interior point with $h'(c)=f'(c)-m=0$. The geometric idea is to remove the average trend and find a horizontal [tangent line](tangent-line.md) in what remains.

**Table of contents**

- [Cauchy mean value theorem](cauchy-mean-value-theorem.md)
- [Endpoint secant-tangent approximation](endpoint-secant-tangent-approximation.md)

## ↑ Ancestors (6)

1. [Calculus](calculus-split.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (103)

- [A cubic root from existence to a quantitative bracket](a-cubic-root-from-existence-to-a-quantitative-bracket.md)
- [Antiderivatives on disconnected domains](antiderivatives-on-disconnected-domains.md)
- [Bounded sequence with vanishing increments need not converge](bounded-sequence-with-vanishing-increments-need-not-converge.md)
- [Cauchy mean value theorem](cauchy-mean-value-theorem.md)
- [Constant of integration](constant-of-integration.md)
- [Cosine fixed-point iteration](cosine-fixed-point-iteration.md)
- [Derivative criterion for monotonicity](derivative-criterion-for-monotonicity.md)
- [Differentiability from continuous partial derivatives](differentiability-from-continuous-partial-derivatives.md)
- [Endpoint secant-tangent approximation](endpoint-secant-tangent-approximation.md)
- [Fundamental theorem of calculus](fundamental-theorem-of-calculus.md)
- [Gaussian autoregressive kernel variance correction](gaussian-autoregressive-kernel-variance-correction.md)
- [Hölder exponent greater than one forces constancy](holder-exponent-greater-than-one-forces-constancy.md)
- [Intermediate secant slope from endpoint derivatives](intermediate-secant-slope-from-endpoint-derivatives.md)
- [Interval bisection](interval-bisection.md)
- [Lipschitz composition preserves Riemann integrability](lipschitz-composition-preserves-riemann-integrability.md)
- [Lipschitz continuity](lipschitz-continuity.md)
- [Local-shift sensitivity](local-shift-sensitivity.md)
- [Locally Lipschitz function](locally-lipschitz-function.md)
- [Mean value theorem](mean-value-theorem.md)
- [Odd-even comparison for Feigenbaum partition lengths](odd-even-comparison-for-feigenbaum-partition-lengths.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/11d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/4d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/1a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/1a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/11a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-55/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/11c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3/16f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-1/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-1/9e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/13f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-85/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/10e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/10e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/3h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/12f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/21g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2/2a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/13f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-75/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2/10f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/13e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/3e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/2f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-64/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/12d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/12f/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/7d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7/2/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-1/11e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-61/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-1/10e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-1/10e/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-1/9d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/12f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/3f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/23j/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/9e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/3g/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-1/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-1/9d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/11g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-105/3/2/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-1/10f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-107/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-327/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-1/10d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/2e/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/9d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/11d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/11d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-107/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/2f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-209/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-105/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-1/11e/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-1/11e/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-166/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-1/10e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-168/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/3/b/solution.md)
- [Radial Schwartz approximation of tempered distributions](radial-schwartz-approximation-of-tempered-distributions.md)
- [Rolle theorem](rolle-theorem.md)
- [Uniform error bound for nearby decaying exponentials](uniform-error-bound-for-nearby-decaying-exponentials.md)
- [Uniform negative curvature and global maximization](uniform-negative-curvature-and-global-maximization.md)
