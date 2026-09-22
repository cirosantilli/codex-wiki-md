<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The negative drift moves the [outflow boundary layer](../../../../../../../outflow-boundary-layer.md) to $x=1$. The first-order outer equation is $-(1+x)y_0'+y_0=0$. It must satisfy the left [boundary condition](../../../../../../../boundary-condition.md), giving $y_0=1+x$. This tends to two at the right endpoint.

Use $X=(1-x)/\epsilon$. The leading inner equation is $Y_0''+2Y_0'=0$, and impose $Y_0(0)=1$ and $Y_0\to2$ on matching. Thus $Y_0=2-e^{-2X}$, and a leading [uniform asymptotic approximation](../../../../../../../uniform-asymptotic-approximation.md) is

$$
\boxed{y\sim1+x-e^{-2(1-x)/\epsilon}}.
$$

For higher accuracy, expand the drift as $2-\epsilon X$ in the inner equation, solve the successive inhomogeneous equations, and match to outer corrections satisfying zero left endpoint data. There is no need for a left endpoint layer. Choosing the growing exponential at the wrong endpoint would prevent matching and is the reason the layer location matters.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 74](../../../../paper-74-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
