<h1 id="p/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the corrected [Hermite interpolating polynomial](../../../../../hermite-interpolating-polynomial.md) from part (a). The auxiliary function $\varphi$ vanishes at all $n+1$ nodes and at the additional point $x$. Its [derivative](../../../../../derivative.md) vanishes at all nodes, because both $e'(x_i)$ and the [derivative](../../../../../derivative.md) of $\pi^2$ vanish there. [Rolle's theorem](../../../../../rolle-theorem.md) between the $n+2$ ordered zeros of $\varphi$ gives $n+1$ further, distinct zeros of $\varphi'$. Thus $\varphi'$ has $2n+2$ distinct zeros on the closed interval. The printed phrase that these include $x$ is not generally true; the extra zeros lie in intervals between zeros of $\varphi$, and $\varphi'(x)$ need not vanish.

Repeated application of [Rolle's theorem](../../../../../rolle-theorem.md) gives $\varphi^{(2n+2)}(\xi)=0$ for some interior $\xi$. Since $h$ has degree at most $2n+1$ and $\pi^2$ is [monic](../../../../../monic-polynomial.md) of degree $2n+2$,

$$
0=f^{(2n+2)}(\xi)-\frac{e(x)}{\pi(x)^2}(2n+2)!.
$$

Rearranging gives

$$
\boxed{e(x)=\frac{f^{(2n+2)}(\xi)}{(2n+2)!}\prod_{i=0}^n(x-x_i)^2.}
$$

At an interpolation node, both sides are zero, so the error formula extends to the whole closed interval. The false location claim about one zero is unnecessary for this result.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
