<h1 id="1/2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The coordinate change has inverse $x=\tilde x-\tilde y^2+\varepsilon$, $y=\tilde y$. Thus the coefficient function needed after changing variables is

$$
\boxed{\tilde f_\varepsilon(\tilde x,\tilde y)=f(\tilde x-\tilde y^2+\varepsilon,\tilde y).}
$$

The PDF's displayed formula has an undefined subscript $f_\alpha$ and writes the forward change in the argument. It is not the coefficient pullback by the stated coordinates; the inverse expression above is the one used in transforming the equation. The forward [polynomial](../../../../../../../polynomial-split.md) composition, if intended instead, has the same type of uniform bounds, but is not that pullback.

For $|(\tilde x,\tilde y)|\le1/2$ and $0\le\varepsilon\le1/32$, the inverse image lies in the fixed compact subset specified by $|x|\le25/32$, $|y|\le1/2$, whose Euclidean radius is less than one. A [real analytic function](../../../../../../../real-analytic-function.md) extends holomorphically to a complex neighborhood of this compact set: local extensions agree on overlaps by uniqueness, and a finite covering gives a common smaller neighborhood. The [polynomial](../../../../../../../polynomial-split.md) inverse maps a fixed small complex neighborhood of the closed half-ball into that neighborhood, uniformly in $\varepsilon$. The extensions are bounded there by a common constant $A$. Applying the multivariable [Cauchy estimate](../../../../../../../cauchy-estimate.md) on equal-radius polydiscs gives

$$
\boxed{\|\partial^\beta\tilde f_\varepsilon\|_\infty\le A\beta!R^{-|\beta|}=\gamma\beta!\zeta^{|\beta|}.}
$$

This is [uniform analyticity under polynomial coordinate changes](../../../../../../../uniform-analyticity-under-polynomial-coordinate-changes.md). The argument gives a compact margin and a common complex radius, not merely separate analyticity for each parameter.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
