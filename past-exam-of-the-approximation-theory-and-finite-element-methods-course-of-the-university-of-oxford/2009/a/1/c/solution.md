<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For uniformly spaced nodes,

$$
\pi_{n,s}(x_s)=h^n\prod_{j\ne s}(s-j)
=(-1)^{n-s}h^ns!(n-s)!.
$$

There are $n-s$ negative factors, coming from $j>s$. Thus the weights fixed by part (b) satisfy this formula exactly. The printed sign $(-1)^s$ agrees for even $n$; for odd $n$ it differs by the common factor $-1$. Rescaling all weights by $(-1)^n$ gives the printed convention without changing the [barycentric interpolation formula](../../../../../barycentric-interpolation-formula.md).

For even $n$, the required magnitude is

$$
\left|\frac{w_0}{w_{n/2}}\right|
=\frac{((n/2)!)^2}{n!}
=\binom n{n/2}^{-1}.
$$

[Stirling's formula](../../../../../stirling-formula.md) gives

$$
\frac{((n/2)!)^2}{n!}
\sim\frac{\pi n(n/(2e))^n}{\sqrt{2\pi n}(n/e)^n}
=\boxed{\frac{\sqrt{\pi n}}{2^{n+1/2}}.}
$$

Thus central weights are exponentially larger in magnitude than endpoint weights. Their alternating signs can cause severe cancellation in polynomial interpolation at equispaced nodes; they reflect the unfavorable high-degree interpolation geometry associated with [Runge's phenomenon](../../../../../runge-s-phenomenon.md). A barycentric evaluation formula improves the implementation but does not remove the intrinsic sensitivity or guarantee convergence for every smooth function. The comparison with the bounded relative weights at [Chebyshev-Lobatto nodes](../../../../../chebyshev-lobatto-node.md) is decisive.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
