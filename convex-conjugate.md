# Convex conjugate

↑ **Parent:** [Convex optimization](convex-optimization-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_conjugate)

The [convex conjugate](convex-conjugate.md) records a [function](function-split.md) using slopes rather than input positions. Let $f:\mathbb R^n\to\mathbb R\cup\{+\infty\}$ be a [proper extended-real function](proper-extended-real-function.md): it is finite somewhere and never takes $-\infty$. Its [convex conjugate](convex-conjugate.md) is

$$
f^*(p)=\sup_{x\in\mathbb R^n}\{p\cdot x-f(x)\}=\sup_{x\in\operatorname{dom}f}\{p\cdot x-f(x)\},\qquad p\in\mathbb R^n,
$$

where $p\cdot x$ is the [dot product](dot-product.md) and $\operatorname{dom}f=\{x:f(x)<+\infty\}$ is the [effective domain](effective-domain.md). An infinite value of $f$ excludes that input from the [supremum](supremum.md). The value $f^*(p)$ can be $+\infty$, but cannot be $-\infty$ because an input with finite $f(x)$ supplies a finite lower bound.

The [convex conjugate](convex-conjugate.md) is automatically a [convex function](convex-function.md), even when $f$ is not [convex](convex-function.md): each fixed input gives an [affine function](affine-function.md) $p\mapsto p\cdot x-f(x)$, and their [supremum](supremum.md) is [convex](convex-function.md). It is also [lower semicontinuous](lower-semicontinuity.md). It need not be proper: for $f(x)=-x^2$ on $\mathbb R$, $px-f(x)=px+x^2$ is unbounded above for every $p$. The definition and the automatic [convexity](convex-function.md) are discussed in [Boyd and Vandenberghe, Convex Optimization (2004), §3.3.1](https://stanford.edu/~boyd/cvxbook/bv_cvxbook.pdf#page=105).

**The best lower bound with a prescribed slope.** Whenever $f^*(p)$ is finite, the [affine function](affine-function.md)

$$
\ell_p(x)=p\cdot x-f^*(p)
$$

is an [affine minorant](affine-minorant.md) of $f$. Indeed, an [affine function](affine-function.md) $p\cdot x+b$ lies below $f$ everywhere exactly when $b\leq\inf_x(f(x)-p\cdot x)=-f^*(p)$. Thus $-f^*(p)$ is the largest possible intercept at slope $p$. The [convex conjugate](convex-conjugate.md) trades positions for slopes: $x$ specifies where to inspect $f$, whereas $p$ specifies which global [affine minorant](affine-minorant.md) to use. Taking the [supremum](supremum.md) over all these [affine minorants](affine-minorant.md) produces the [biconjugate](biconjugate.md); the [Fenchel-Moreau theorem](fenchel-moreau-theorem.md) says this recovers a [proper convex function](proper-convex-function.md) when it is [lower semicontinuous](lower-semicontinuity.md).

**A quadratic, computed by completing the square.** For the [convex quadratic function](convex-quadratic-function.md) $f(x)=x^2/2$,

$$
px-\frac{x^2}{2}=\frac{p^2}{2}-\frac{(x-p)^2}{2}.
$$

Consequently $f^*(p)=p^2/2$, and the unique maximizing input is $x=p$. The [affine minorant](affine-minorant.md) $\ell_p(x)=px-p^2/2$ is the [tangent line](tangent-line.md) at $(p,p^2/2)$: its slope is $p$ and its intercept is $-f^*(p)=-p^2/2$. For example, $p=2$ gives $f^*(2)=2$ and the [tangent line](tangent-line.md) $2x-2$, touching at $(2,2)$. This is the same curve described either by its point values or by the intercepts of its [tangent lines](tangent-line.md).

<a id="image-the-convex-conjugate-determines-the-intercept-of-each-tangent-line-of-a-convex-quadratic-function"></a>
![](convex-conjugate-support-lines.png)

**[Figure 9](#image-the-convex-conjugate-determines-the-intercept-of-each-tangent-line-of-a-convex-quadratic-function). The convex conjugate determines the intercept of each tangent line of a convex quadratic function**. For the [convex quadratic function](convex-quadratic-function.md) $f(x)=x^2/2$, the colored [tangent lines](tangent-line.md) have slopes $p=-1,0,2$ and touch at $x=p$. The right panel plots the [convex conjugate](convex-conjugate.md) $f^*(p)=p^2/2$ and marks the matching slope-value pairs. The highlighted [tangent line](tangent-line.md) $2x-2$ has intercept $-f^*(2)=-2$.

**A corner turns into a constraint on slopes.** For the [absolute value](absolute-value.md) $f(x)=|x|$, if $|p|\leq1$ then $px-|x|\leq0$, with value zero at $x=0$. If $p>1$, taking $x\to+\infty$ makes $(p-1)x\to+\infty$; if $p<-1$, taking $x\to-\infty$ does the same. Therefore its [convex conjugate](convex-conjugate.md) is zero on $[-1,1]$ and $+\infty$ outside: it is the [indicator functional of a constraint set](indicator-functional-of-a-constraint-set.md) for this interval. For $|p|<1$ the unique maximizing input is zero; for $p=1$ every $x\geq0$ maximizes, and for $p=-1$ every $x\leq0$ maximizes. The corner's many supporting slopes are exactly the [subdifferential](subdifferential.md) $\partial f(0)=[-1,1]$.

**A supremum need not be attained.** For a [differentiable](differentiable-function.md) [convex function](convex-function.md) finite on all of $\mathbb R^n$, an input maximizes $p\cdot x-f(x)$ exactly when $p=\nabla f(x)$. If $f$ is [strictly convex](strictly-convex-function.md), there is at most one such input; existence is a separate issue. For the [exponential function](exponential-function.md) $f(x)=e^x$, the [derivative](derivative.md) is positive. At $p>0$, solving $p=e^x$ gives $x=\log p$ and $f^*(p)=p\log p-p$. At $p=0$, the [supremum](supremum.md) of $-e^x$ is zero as $x\to-\infty$, with no maximizing input. At $p<0$, $px-e^x\to+\infty$ as $x\to-\infty$. Thus a [strictly convex](strictly-convex-function.md) [differentiable](differentiable-function.md) [function](function-split.md) can have both unattained finite conjugate values and infinite conjugate values.

**Table of contents**

- [Utility conjugate](utility-conjugate.md)
  - [Dual differentiability with nonvanishing utility curvature](dual-differentiability-with-nonvanishing-utility-curvature.md)
- [Convex conjugate of x log x](convex-conjugate-of-x-log-x.md)
- [Biconjugate](biconjugate.md)
- [Affine covariance of the convex conjugate](affine-covariance-of-the-convex-conjugate.md)
- [Concave Legendre dual](concave-legendre-dual.md)
  - [Lower conjugate](lower-conjugate.md)
    - [Concave biconjugate](concave-biconjugate.md)
  - [Inverse-flux quadratic bounds](inverse-flux-quadratic-bounds.md)
- [Convex conjugate of a constrained quadratic](convex-conjugate-of-a-constrained-quadratic.md)
- [Fenchel-Moreau theorem](fenchel-moreau-theorem.md)
  - [Biconjugation as closed convexification](biconjugation-as-closed-convexification.md)
- [Fenchel–Young inequality](fenchel-young-inequality.md)
  - [Fenchel–Young gap](fenchel-young-gap.md)

## ↑ Ancestors (5)

1. [Convex optimization](convex-optimization-split.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (39)

- [Affine covariance of the convex conjugate](affine-covariance-of-the-convex-conjugate.md)
- [Biconjugate](biconjugate.md)
- [Chambolle–Pock algorithm](chambolle-pock-algorithm.md)
- [Concave Legendre dual](concave-legendre-dual.md)
- [Conjugate of the squared distance to a convex set](conjugate-of-the-squared-distance-to-a-convex-set.md)
- [Convex analysis](convex-analysis.md)
- [Convex conjugate](convex-conjugate.md)
- [Convex conjugate of x log x](convex-conjugate-of-x-log-x.md)
- [Fenchel–Young gap](fenchel-young-gap.md)
- [Fenchel–Young inequality](fenchel-young-inequality.md)
- [Infimal convolution](infimal-convolution.md)
- [Legendre dual cone barrier](legendre-dual-cone-barrier.md)
- [Lower conjugate](lower-conjugate.md)
- [Moreau decomposition](moreau-decomposition.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-50/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/4c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-68/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326/3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326/3/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326/3/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326/3/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326/3/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-348/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-339/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-339/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-339/2/c/solution.md)
- [Reuss elastic approximation](reuss-elastic-approximation.md)
- [Support function](support-function.md)
