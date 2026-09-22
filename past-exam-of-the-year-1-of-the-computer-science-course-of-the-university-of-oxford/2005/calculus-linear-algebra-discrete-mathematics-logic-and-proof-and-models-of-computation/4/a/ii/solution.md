<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [product rule](../../../../../../product-rule.md) for the [Laplace operator](../../../../../../laplace-operator.md):

$$
\Delta(xg(r))=x\Delta g(r)+2\partial_xg(r)=x\left(g''+\frac{g'}r\right)+2\frac{x}{r}g'=x\left(g''+\frac{3g'}r\right).
$$

Thus [Laplace's equation](../../../../../../laplace-equation.md), away from the origin, reduces to $g''+3g'/r=0$. On the line $x=0$ the displayed expression vanishes automatically; requiring the equation on an open region gives the same radial equation by continuity from $x\ne0$. Multiplying by $r^3$ gives $(r^3g')'=0$, so $g'=Cr^{-3}$ and $g=A+Br^{-2}$. Therefore

$$
\boxed{u(x,y)=Ax+B\frac{x}{x^2+y^2},\qquad r>0.}
$$

If extension through the origin is required, $B=0$: along the horizontal axis the second term is $B/x$. The remaining [harmonic function](../../../../../../harmonic-function.md) is $Ax$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
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
