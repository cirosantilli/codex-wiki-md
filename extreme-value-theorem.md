# Extreme value theorem

↑ **Parent:** [Real analysis](real-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Extreme_value_theorem)

A [real-valued function](real-valued-function.md) that is [continuous](continuous-function.md) on a nonempty [compact space](compact-space.md) attains both a [global minimum](global-minimum.md) and a [global maximum](global-maximum.md). In particular, for a [continuous function](continuous-function.md) $f:[a,b]\to\mathbb R$ on a nonempty [closed interval](closed-real-interval.md), there are points $x_{\min},x_{\max}\in[a,b]$ such that

$$
f(x_{\min})\leq f(x)\leq f(x_{\max})
\qquad\text{for every }x\in[a,b].
$$

The important word is “attains”: the best values occur at actual allowed inputs, rather than merely being approached. The interval version is [Jiří Lebl, Basic Analysis I, theorem 3.3.2](https://jirilebl.github.io/ra/html/sec_minmaxint.html).

For a worked example, take $f(x)=(x-1)^2$ on $[-1,2]$. Its [global minimum](global-minimum.md) is $f(1)=0$, and its [global maximum](global-maximum.md) is $f(-1)=4$. Nonnegativity gives the first answer; $|x-1|\leq2$ on the specified [closed interval](closed-real-interval.md) gives the second. The endpoint $x=-1$ is essential: looking only for a zero [derivative](derivative.md) would find the minimum and miss the maximum.

<a id="image-an-attained-minimum-and-maximum-on-a-closed-interval-compared-with-excluded-endpoints-and-a-discontinuous-endpoint-value"></a>
![](extreme-value-theorem-attainment.png)

**[Figure 16](#image-an-attained-minimum-and-maximum-on-a-closed-interval-compared-with-excluded-endpoints-and-a-discontinuous-endpoint-value). An attained minimum and maximum on a closed interval, compared with excluded endpoints and a discontinuous endpoint value**.

For comparison, the [continuous function](continuous-function.md) $g(x)=x$ on the [open interval](open-interval.md) $(0,1)$ has [infimum](infimum.md) $0$ and [supremum](supremum.md) $1$, but neither is a value of $g$. Even a closed domain is insufficient without [continuity](continuous-function.md): define $h(x)=x$ for $0\leq x<1$, and $h(1)=0$. On $[0,1]$, its [supremum](supremum.md) is $1$, approached by $x_n=1-1/n$ for $n\geq2$, but every function value is strictly less than $1$. This endpoint change makes $h$ [discontinuous](discontinuity-of-a-function.md), preventing attainment. On the unbounded [real line](real-line.md), the [continuous function](continuous-function.md) $x\mapsto x$ has neither a [global minimum](global-minimum.md) nor a [global maximum](global-maximum.md). These examples show what can fail when a hypothesis is dropped; functions outside the hypotheses may still have extrema.

The [extreme value theorem](extreme-value-theorem.md) is an existence tool for [optimization](mathematical-optimization-split.md): first establish that a [continuous](continuous-function.md) [objective function](objective-function.md) on a nonempty [compact](compact-space.md) [feasible set](feasible-region.md) has a best value, then investigate where it occurs. It neither locates the optimizing point nor promises uniqueness or [differentiability](differentiability.md). For example, the [absolute value](absolute-value.md) function $|x|$ on $[-1,2]$ has its [global minimum](global-minimum.md) at zero although no [derivative](derivative.md) exists there; a [constant function](constant-function.md) has every input as a [minimizer](global-minimizer.md). This role in [optimization](mathematical-optimization-split.md) is explained in [University of Toronto MAT237 notes, section 1.4: compactness and the extreme value theorem](https://www.math.utoronto.ca/courses/mat237y1/20189/notes/Chapter1/S1.4.html).

A short proof outline identifies the mechanism. The [continuous image of a compact space](continuous-image-of-a-compact-space.md) is [compact](compact-space.md); a nonempty [compact subset](compact-space.md) of the [real line](real-line.md) contains its [infimum](infimum.md) and [supremum](supremum.md). For a [closed interval](closed-real-interval.md), one can instead choose inputs whose outputs approach the [supremum](supremum.md), extract a convergent [subsequence](subsequence.md) by the [Bolzano-Weierstrass theorem](bolzano-weierstrass-theorem.md), and use [continuity](continuous-function.md) to make its limiting output equal that [supremum](supremum.md). The [closed interval](closed-real-interval.md) retains the limiting input. Repeating the argument for the [infimum](infimum.md) supplies the minimum.

**Table of contents**

- [Interior-value criterion for an attained maximum](interior-value-criterion-for-an-attained-maximum.md)
- [Supremum can fail to be attained at an oscillatory endpoint](supremum-can-fail-to-be-attained-at-an-oscillatory-endpoint.md)

## ↑ Ancestors (5)

1. [Real analysis](real-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (58)

- [Bolzano-Weierstrass theorem](bolzano-weierstrass-theorem.md)
- [Closed real interval](closed-real-interval.md)
- [Compact space](compact-space.md)
- [Continuous function](continuous-function.md)
- [Continuous image of a compact space](continuous-image-of-a-compact-space.md)
- [Convex optimization](convex-optimization-split.md)
- [Empty and open feasible regions](empty-and-open-feasible-regions.md)
- [Extreme value theorem](extreme-value-theorem.md)
- [Feasible point](feasible-point.md)
- [Finite-valued infimal convolution](finite-valued-infimal-convolution.md)
- [Global minimum](global-minimum.md)
- [Interior-value criterion for an attained maximum](interior-value-criterion-for-an-attained-maximum.md)
- [Lipschitz composition preserves Riemann integrability](lipschitz-composition-preserves-riemann-integrability.md)
- [Local maximum of Brownian motion](local-maximum-of-brownian-motion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/4d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4/1a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/12c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/11b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-1/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/14f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/11e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-1/10d/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/10d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/11d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/10f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/3e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/1/1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/10d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/10d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/2i/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/9e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-1/9d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-1/9f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-2/12f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-2/12f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/2f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-339/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/2h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/10d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/11d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/12f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/12f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-133/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/20/c/solution.md)
- [Peano existence theorem](peano-existence-theorem.md)
- [Range of a continuous coercive real function](range-of-a-continuous-coercive-real-function.md)
- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
- [Rolle theorem](rolle-theorem.md)
- [Supremum can fail to be attained at an oscillatory endpoint](supremum-can-fail-to-be-attained-at-an-oscillatory-endpoint.md)
- [Supremum norm](supremum-norm.md)
