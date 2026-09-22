<h1 id="6a/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The defining [Wronskian](../../../../../../../wronskian.md) identity gives the [first-order linear differential equation](../../../../../../../first-order-linear-differential-equation.md)

$$
\boxed{y_2'-\frac{y_1'}{y_1}y_2=\frac{W}{y_1}.}
$$

Work first on an interval where $y_1\ne0$. Dividing by $y_1$ recognizes a [derivative](../../../../../../../derivative.md):

$$
\left(\frac{y_2}{y_1}\right)'=\frac{W}{y_1^2},\qquad \boxed{y_2(x)=y_1(x)\left(C+\int_{x_0}^x\frac{W(s)}{y_1(s)^2}\,ds\right).}
$$

This is [reduction of order](../../../../../../../reduction-of-order.md). Choose the nonzero [Wronskian](../../../../../../../wronskian.md) from the [Abel identity](../../../../../../../abel-s-identity.md) to obtain [linear independence](../../../../../../../linear-independence.md). The constant $C$ only adds a multiple of $y_1$. If $y_1$ has zeros, this quotient formula is local; the resulting solution can be continued across ordinary zeros using the original [second-order linear differential equation](../../../../../../../second-order-linear-differential-equation.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6A](../../../6a.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
