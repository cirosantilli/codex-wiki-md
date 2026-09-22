<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Parametrize the line as $\ell(t)=x+t(x'-x)$ and set $F(t)=f(\ell(t))$, a polynomial of degree at most three. The [Jacobian criterion](../../../../../../jacobian-criterion.md) at a singular point of a hypersurface gives vanishing of its equation and all first derivatives. Consequently

$$
F(0)=F(1)=0,\qquad
F'(0)=\sum_j(x'_j-x_j)f_{t_j}(x)=0,\qquad
F'(1)=\sum_j(x'_j-x_j)f_{t_j}(x')=0.
$$

Thus $t^2$ and $(t-1)^2$ both divide $F$. They are coprime in every characteristic, so their degree-four product divides a polynomial of degree at most three. It follows that $F=0$, proving

$$
\boxed{\ell(\mathbb A^1)\subseteq X.}
$$

This is the [secant line through singular points of a cubic hypersurface](../../../../../../secant-line-through-singular-points-of-a-cubic-hypersurface.md) argument. If the given defining polynomial has repeated factors, use its square-free part for the reduced variety's Jacobian criterion: vanishing of that polynomial and its gradient at a singular point implies vanishing of the original polynomial's gradient there as well, by the product rule. The same restriction argument therefore still applies.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
