<h1 id="1a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Divide the [second-order difference equation](../../../../../../second-order-difference-equation.md) by $h^2$ and set $x=nh$. The first quotient is a [central finite difference](../../../../../../central-finite-difference.md) approximation to $y''(x)$; the quotient $(y_{n+1}-y_{n-1})/(2h)$ approximates $y'(x)$. Their [Taylor series](../../../../../../taylor-series.md) errors are $O(h^2)$ for a sufficiently smooth function. This is therefore a [finite difference method](../../../../../../finite-difference-method.md) for the [second-order linear differential equation](../../../../../../second-order-linear-differential-equation.md) in part (a).

At a fixed $x\geq0$, take $h\to0$ with $n=x/h$ integral. Since $\log r_-=-2h+O(h^3)$, the exact bounded discrete solution satisfies

$$
\boxed{r_-^{x/h}=\exp\bigl(-2x+O(xh^2)\bigr)\longrightarrow e^{-2x}.}
$$

Likewise $(1-2h)^{x/h}\to e^{-2x}$. The decay selected by boundedness in the [linear recurrence relation](../../../../../../linear-recurrence-relation.md) becomes exactly the decay selected by boundedness in the [ordinary differential equation](../../../../../../ordinary-differential-equation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1A](../../1a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
