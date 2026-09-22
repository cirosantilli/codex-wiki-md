<h1 id="m/m3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For sufficiently large $n$, $p_n=\lambda/n$ lies in $(0,1]$. The waiting time has the [geometric distribution](../../../../../geometric-distribution.md) on $1,2,\ldots$, so summing its [geometric series](../../../../../geometric-series.md) gives

$$
M_{Y_n/n}(t)=\sum_{j=1}^\infty p_n(1-p_n)^{j-1}e^{tj/n}
=\boxed{\frac{(\lambda/n)e^{t/n}}{1-(1-\lambda/n)e^{t/n}}},
$$

whenever $(1-\lambda/n)e^{t/n}<1$. Fix $t<\lambda$. The expansions $e^{t/n}=1+t/n+O(n^{-2})$ show that the numerator is $\lambda/n+O(n^{-2})$ and the denominator is $(\lambda-t)/n+O(n^{-2})$. Therefore

$$
M_{Y_n/n}(t)\longrightarrow\frac\lambda{\lambda-t}.
$$

The [convergence theorem for moment-generating functions](../../../../../convergence-theorem-for-moment-generating-functions.md) says that pointwise convergence of finite [moment-generating functions](../../../../../moment-generating-function.md) on a fixed open interval about zero to the [moment-generating function](../../../../../moment-generating-function.md) of a [probability distribution](../../../../../probability-distribution-split.md) implies [convergence in distribution](../../../../../convergence-in-distribution.md) to that distribution. For example take $|t|<\lambda/2$; all large $n$ satisfy the convergence condition throughout that interval. The limit is the [moment-generating function](../../../../../moment-generating-function.md) from part (a), proving

$$
\boxed{Y_n/n\xrightarrow{d}\operatorname{Exp}(\lambda)}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [M3](../../m3.md)
3. [M](../../../m.md)
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
