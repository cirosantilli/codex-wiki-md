<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $y_1=e^x/x$, on an [interval](../../../../../../interval-mathematics.md) avoiding zero,

$$
y_1'=e^x\left(\frac1x-\frac1{x^2}\right),\qquad y_1''=e^x\left(\frac1x-\frac2{x^2}+\frac2{x^3}\right).
$$

Substitution into the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) gives

$$
xy_1''+2y_1'-xy_1=e^x\left(1-\frac2x+\frac2{x^2}+\frac2x-\frac2{x^2}-1\right)=0.
$$

To find an independent solution, put $v=xy$. The [product rule](../../../../../../product-rule.md) gives $v''=xy''+2y'$, so the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) becomes $v''-v=0$. Its independent solutions are $e^x$ and $e^{-x}$. Hence

$$
\boxed{y_2(x)=\frac{e^{-x}}x,\qquad y(x)=\frac{Ae^x+Be^{-x}}x\quad(x\ne0).}
$$

The two displayed solutions are [linearly independent](../../../../../../linear-independence.md), since their ratio $e^{2x}$ is nonconstant on any open [interval](../../../../../../interval-mathematics.md). Constants can be chosen separately on the two sides of the singular point $x=0$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2005](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
