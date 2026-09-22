<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Because $f$ is a [compactly supported distribution](../../../../../compactly-supported-distribution.md), the [convolution of distributions with a compactly supported factor](../../../../../convolution-of-distributions-with-a-compactly-supported-factor.md) defines $E*f$. The [convolution derivative identity](../../../../../differentiation-commutes-with-convolution.md) and part (i) give

$$
\partial_{\bar z}(E*f)=(\partial_{\bar z}E)*f=\delta_0*f=f.
$$

The difference between any two solutions has zero $\partial_{\bar z}$ [distributional derivative](../../../../../distributional-derivative.md). Part (ii) therefore proves that the general solution of the [partial differential equation](../../../../../partial-differential-equation-split.md) is

$$
\boxed{u=\left(\frac1{\pi z}\right)*f+h,\qquad h\text{ any entire function}.}
$$

This formula is an identity of [distributions](../../../../../distribution-mathematical-analysis.md); a pointwise integral is not required for arbitrary $f$.

If $u$ were a [smooth function](../../../../../smooth-function.md), its [Wirtinger derivative](../../../../../wirtinger-derivatives.md) $\partial_{\bar z}u=f$ would also be smooth, contradicting $\operatorname{sing\,supp}f\ne\varnothing$. In fact the [singular support](../../../../../singular-support.md) is exactly preserved here:

$$
\boxed{\operatorname{sing\,supp}u=\operatorname{sing\,supp}f.}
$$

One inclusion follows because a [differential operator](../../../../../differential-operator.md) cannot create a singularity where $u$ is smooth. For the reverse inclusion, $E$ is smooth off zero, and its [singular support](../../../../../singular-support.md) is exactly $\{0\}$: if it were smooth near zero, $\partial_{\bar z}E=\delta_0$ would be smooth there. The [support and singular support rules for convolution](../../../../../support-and-singular-support-rules-for-convolution.md) give $\operatorname{sing\,supp}(E*f)\subseteq\{0\}+\operatorname{sing\,supp}f$, and adding the smooth [entire function](../../../../../entire-function.md) $h$ leaves this [singular support](../../../../../singular-support.md) unchanged. Thus there is no globally smooth solution when the given [singular support](../../../../../singular-support.md) is nonempty.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
