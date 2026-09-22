<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [d](../d.md)

Let $F=e^g$. It is [holomorphic](../../../../holomorphic-function-split.md) and nowhere zero on a punctured neighbourhood of $a$, and the [chain rule](../../../../chain-rule.md) gives

$$
\frac{F'}F=g'.
$$

If $F$ had a [pole](../../../../pole.md) of order $n\geq1$, part (c) would imply $\operatorname{Res}_a(g')=-n$. But the derivative of a [holomorphic function](../../../../holomorphic-function-split.md) on a punctured disc has [residue](../../../../residue.md) zero. Indeed, write its [Laurent series](../../../../laurent-series.md)

$$
g(z)=\sum_{k\in\mathbb Z}c_k(z-a)^k,\qquad g'(z)=\sum_{k\in\mathbb Z}k c_k(z-a)^{k-1}.
$$

Termwise differentiation is valid on every smaller closed annulus. The only possible $(z-a)^{-1}$ term comes from $k=0$ and has coefficient zero. Thus

$$
\boxed{\operatorname{Res}_a(g')=0\ne-n},
$$

a contradiction. Therefore $\boxed{e^g\text{ cannot have a pole at }a}$. This proves [an exponential has no isolated pole](../../../../an-exponential-has-no-isolated-pole.md), including when $g$ has an [essential singularity](../../../../essential-singularity.md); no choice of a [holomorphic logarithm](../../../../holomorphic-logarithm.md) on the entire punctured disc was assumed.

## ↑ Ancestors (12)

1. [d](../d.md)
2. [4](../../4.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
