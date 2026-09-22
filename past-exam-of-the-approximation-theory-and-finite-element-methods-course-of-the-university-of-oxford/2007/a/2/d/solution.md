<h1 id="a/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [polynomial](../../../../../polynomial-split.md) $T_6$ is

$$
T_6(x)=32x^6-48x^4+18x^2-1.
$$

Subtract its monic version from $x^6$:

$$
\boxed{p(x)=x^6-\frac1{32}T_6(x)
=\frac32x^4-\frac9{16}x^2+\frac1{32}.}
$$

This has degree four and hence belongs to the usual space $P_5$. The error is $T_6/32$, with [norm](../../../../../norm.md) $1/32$ and alternating extrema at the seven points $\cos(j\pi/6)$, $j=0,\ldots,6$. Part (a), followed by [uniqueness](../../../../../uniqueness.md), proves

$$
\boxed{\|x^6-p\|_\infty=\frac1{32}}
$$

and that this is the unique [best approximation](../../../../../best-approximation-in-a-normed-space.md) of degree at most five.

If “degree five” is taken literally to exclude degree four, no [best approximation](../../../../../best-approximation-in-a-normed-space.md) exists in that nonclosed class: $p+\epsilon x^5$ approaches the error $1/32$ as $\epsilon\to0$, but [uniqueness](../../../../../uniqueness.md) in $P_5$ excludes attainment by any degree-five [polynomial](../../../../../polynomial-split.md). This is why the standard at-most-degree convention matters here.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
