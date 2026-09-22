<h1 id="2/a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [Weierstrass M-test](../../../../../weierstrass-m-test.md) proof of the [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md), the required bound is

$$
\boxed{Mh\leq k,\qquad\text{with no additional restriction on }Lh.}
$$

To see this, use [Picard iteration](../../../../../picard-iteration.md) starting with $y_0(x)=b$ and

$$
y_{n+1}(x)=b+\int_a^x f(s,y_n(s))\,ds.
$$

If $y_n$ takes its values in $[b-k,b+k]$, then $|y_{n+1}-b|\leq M|x-a|\leq Mh\leq k$. Thus every [Picard iterate](../../../../../picard-iterate.md) remains in the rectangle where the hypotheses hold. Successive applications of the [Lipschitz condition](../../../../../lipschitz-continuity.md) and [integration](../../../../../integral-split.md) give the [factorial estimate for Picard iteration](../../../../../factorial-estimate-for-picard-iteration.md)

$$
|y_{n+1}(x)-y_n(x)|\leq\frac{ML^n|x-a|^{n+1}}{(n+1)!}.
$$

For example, the $n=0$ estimate is $M|x-a|$, and integrating the $n$th estimate multiplied by $L$ proves the next one. The sum of the uniform bounds is

$$
\sum_{n=0}^{\infty}\frac{ML^nh^{n+1}}{(n+1)!}<\infty
$$

for every finite $Lh$, by the [exponential series](../../../../../exponential-series.md). Hence the telescoping series of [Picard iterates](../../../../../picard-iterate.md) converges uniformly by the [Weierstrass M-test](../../../../../weierstrass-m-test.md). The [uniform limit](../../../../../uniform-limit.md) stays in the closed rectangle, and the [Lipschitz condition](../../../../../lipschitz-continuity.md) permits passage to the limit in the [integral equation](../../../../../integral-equation.md). The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) then gives the desired [solution of a differential equation](../../../../../solution-of-a-differential-equation.md) on $[a-h,a+h]$.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
