<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By the definition of [little o notation](../../../../little-o-notation.md), the required quotient is

$$
\frac{\epsilon^2\log\epsilon}{\epsilon}=\epsilon\log\epsilon.
$$

As $\epsilon\to0^+$, write this as $\log\epsilon/(1/\epsilon)$. [L'Hôpital's rule](../../../../l-hopital-s-rule.md) applies to this infinite-over-infinite ratio and gives

$$
\lim_{\epsilon\to0^+}\frac{\log\epsilon}{1/\epsilon}
=\lim_{\epsilon\to0^+}\frac{1/\epsilon}{-1/\epsilon^2}
=\lim_{\epsilon\to0^+}(-\epsilon)=0.
$$

Therefore **$\epsilon^2\log\epsilon=o(\epsilon)$**. The [logarithm](../../../../logarithm.md) is negative on this approach, which is consistent with a quotient tending to zero from below; [little o notation](../../../../little-o-notation.md) concerns the limiting ratio, not its sign.[§2.1(i), equation 2.1.2](../../../../nist-digital-library-of-mathematical-functions/2-1-definitions-and-elementary-properties.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
