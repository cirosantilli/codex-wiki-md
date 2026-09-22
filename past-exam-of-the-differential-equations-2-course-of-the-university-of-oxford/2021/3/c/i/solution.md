<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Setting $\epsilon=0$ gives the reduced [first-order linear differential equation](../../../../../first-order-linear-differential-equation.md) $y'=y$. Its nonzero solutions cannot satisfy the zero value at $x=2$, so one endpoint needs a [boundary layer](../../../../../boundary-layer.md). To determine which endpoint, freeze the coefficient at $x=x_b>0$ in the rapidly varying part: $\epsilon y''-x_by'=0$ has fast mode $e^{x_b(x-x_b)/\epsilon}$. It decays into the interval from the right endpoint but grows into the interval from the left endpoint. Hence

$$
\boxed{\text{the boundary layer is at }x=2,\text{ with thickness }O(\epsilon).}
$$

The [dominant balance](../../../../../dominant-balance.md) $\epsilon/\delta^2\sim x_b/\delta$ gives $\delta\sim\epsilon/x_b$, so a convenient local thickness is $\epsilon/2$. The left [boundary condition](../../../../../boundary-condition.md) must select the [outer solution](../../../../../outer-expansion.md). Equivalently, a putative left [inner variable](../../../../../inner-variable.md) $X=(x-1)/\epsilon$ would give $Y_{XX}-Y_X=0$, whose nonconstant solution grows like $e^X$ and cannot satisfy the [asymptotic matching condition](../../../../../asymptotic-matching-condition.md) as $X\to\infty$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
