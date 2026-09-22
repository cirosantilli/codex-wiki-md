<h1 id="8a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\xi=x$ and $\eta=y-1$. The [polynomial](../../../../../../polynomial-split.md) becomes

$$
g=-\xi^3(1+\eta)^2(\xi+\eta)
=-\xi^4-\xi^3\eta+O\bigl((|\xi|+|\eta|)^5\bigr).
$$

There are no terms of degree one or two, so the [gradient](../../../../../../gradient.md) and the entire [Hessian matrix](../../../../../../hessian-matrix.md) vanish at $(0,1)$. It is a [critical point](../../../../../../critical-point.md) with singular [Hessian matrix](../../../../../../hessian-matrix.md). **The lowest nontrivial approximation is**

$$
\boxed{g(x,y)\sim-x^3\bigl(x+(y-1)\bigr),}
$$

understood as the fourth-degree leading term rather than a uniform ratio asymptotic along its zero directions.

On the path $\eta=0$ the exact value is $-\xi^4<0$ for $\xi\ne0$. On the path $\eta=-2\xi$ it is $\xi^4(1-2\xi)^2>0$ for sufficiently small nonzero $\xi$. Both paths approach the point, where $g=0$. **It is neither a [local maximum](../../../../../../local-maximum.md) nor a [local minimum](../../../../../../local-minimum.md); it is a degenerate saddle point of a scalar function.** The [higher-order saddle test](../../../../../../higher-order-saddle-test.md) supplies the conclusion the singular [Hessian matrix](../../../../../../hessian-matrix.md) cannot supply.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8A](../../8a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
