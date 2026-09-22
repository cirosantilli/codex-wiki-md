<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Seek an outer [asymptotic expansion](../../../../../../asymptotic-expansion.md) $y=y_0+\epsilon y_1+\cdots$ for fixed $x>0$. The leading equation is $xy_0'=0$, and the endpoint condition gives $y_0=1$. At first order, $xy_1'=y_0=1$ and $y_1(1)=0$, so $y_1=\log x$. This outer correction cannot be evaluated at $x=0$.

The coefficient $x+\epsilon$ selects the [boundary layer](../../../../../../boundary-layer.md) coordinate $X=x/\epsilon$. With $Y(X)=y(\epsilon X)$, the equation becomes $(1+X)Y_X=\epsilon Y$. Its inner leading term is constant; matching it to the outer solution gives $Y_0=1$. At first order, $Y_{1X}=1/(1+X)$, hence $Y_1=\log(1+X)+C$. In the overlap $1\ll X\ll\epsilon^{-1}$, the outer solution is $1+\epsilon\log\epsilon+\epsilon\log X$. Matching the constants therefore gives

$$
Y(X)=1+\epsilon\log\epsilon+\epsilon\log(1+X)+o(\epsilon)
$$

for fixed $X$. The [logarithmic matching in a small-exponent boundary layer](../../../../../../logarithmic-matching-in-a-small-exponent-boundary-layer.md) must retain $\epsilon\log\epsilon$, which is larger in magnitude than a plain order-$\epsilon$ term. At the endpoint,

$$
\boxed{y(0)=1+\epsilon\log\epsilon+o(\epsilon).}
$$

The coefficient of a separate plain $\epsilon$ term is zero.

Direct integration provides the exact check:

$$
\boxed{y(x;\epsilon)=\left(\frac{x+\epsilon}{1+\epsilon}\right)^\epsilon.}
$$

At zero its logarithm is $\epsilon\log\epsilon-\epsilon\log(1+\epsilon)=\epsilon\log\epsilon-\epsilon^2+O(\epsilon^3)$. Exponentiating gives $y(0)=1+\epsilon\log\epsilon+O(\epsilon^2\log^2\epsilon)$, whose remainder is indeed $o(\epsilon)$. The first-order uniform composite $1+\epsilon\log[(x+\epsilon)/(1+\epsilon)]$ also satisfies the [boundary condition](../../../../../../boundary-condition.md) exactly and reproduces both expansions to the requested order.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
