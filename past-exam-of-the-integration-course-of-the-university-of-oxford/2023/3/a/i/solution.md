<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Minkowski inequality](../../../../../minkowski-inequality.md) states that on a [measure space](../../../../../measure-space.md) $(X,\Sigma,\mu)$, for $1\leq p\leq\infty$ and measurable real or complex $f,g$ of finite [Lp norm](../../../../../lp-norm.md),

$$
\boxed{\|f+g\|_p\leq\|f\|_p+\|g\|_p.}
$$

For $p=1$, integrate the scalar [triangle inequality](../../../../../triangle-inequality.md) $|f+g|\leq|f|+|g|$. For $p=\infty$, the [almost everywhere](../../../../../almost-everywhere.md) bounds $|f|\leq\|f\|_\infty$ and $|g|\leq\|g\|_\infty$ give the same result by taking the [essential supremum](../../../../../essential-supremum.md).

For $1<p<\infty$, first ensure that the left side is finite. The [convex function](../../../../../convex-function.md) $s\mapsto s^p$ on $[0,\infty)$ gives

$$
|f+g|^p\leq(|f|+|g|)^p\leq2^{p-1}(|f|^p+|g|^p),
$$

so $f+g$ has finite [Lp norm](../../../../../lp-norm.md). Set $q=p/(p-1)$ and $H=\|f+g\|_p$. Since $(p-1)q=p$, [Holder inequality](../../../../../holder-inequality.md) gives

$$
H^p\leq\int_X(|f|+|g|)|f+g|^{p-1}\,d\mu
\leq(\|f\|_p+\|g\|_p)\left(\int_X|f+g|^p\,d\mu\right)^{1/q}
=(\|f\|_p+\|g\|_p)H^{p-1}.
$$

If $H=0$ the result is immediate; otherwise divide by $H^{p-1}$. This proves the [triangle inequality](../../../../../triangle-inequality.md) for every claimed exponent.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
