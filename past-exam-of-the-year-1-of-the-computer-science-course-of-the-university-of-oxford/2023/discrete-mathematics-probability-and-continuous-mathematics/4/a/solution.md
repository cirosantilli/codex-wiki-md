<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\mathbf h=\mathbf y-\mathbf x$. For $0<t\le1$, [convexity](../../../../../convex-function.md) gives $f(\mathbf x+t\mathbf h)\le(1-t)f(\mathbf x)+tf(\mathbf y)$, hence

$$
f(\mathbf y)-f(\mathbf x)\ge\frac{f(\mathbf x+t\mathbf h)-f(\mathbf x)}{t}.
$$

By the first-order form of [Taylor's theorem](../../../../../taylor-s-theorem.md), the right side tends to $\mathbf h^{\mathsf T}\nabla f(\mathbf x)$ as $t\downarrow0$. Therefore

$$
\boxed{f(\mathbf y)\ge f(\mathbf x)+(\mathbf y-\mathbf x)^{\mathsf T}\nabla f(\mathbf x).}
$$

This is the [supporting inequality for a differentiable convex function](../../../../../supporting-inequality-for-a-differentiable-convex-function.md). The stated [partial derivatives](../../../../../partial-derivative.md) are enough: [coordinate derivatives give directional Taylor expansion for convex functions](../../../../../coordinate-derivatives-give-directional-taylor-expansion-for-convex-functions.md), so no unmentioned continuity assumption on the second [partial derivatives](../../../../../partial-derivative.md) is needed. The result in fact needs less smoothness than the question assumes.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
