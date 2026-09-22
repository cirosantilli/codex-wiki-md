<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $w_s=1/\pi_{n,s}(x_s)$, the [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) can be written, away from its nodes,

$$
p_n(x)=\pi_n(x)\sum_{s=0}^n\frac{w_su_s}{x-x_s}.
$$

Apply the same formula to the constant data $u_s=1$. Uniqueness of [polynomial interpolation](../../../../../polynomial-interpolation.md) gives $\sum_s\ell_s=1$, and hence

$$
1=\pi_n(x)\sum_{s=0}^n\frac{w_s}{x-x_s}.
$$

Divide the two identities to obtain the [barycentric interpolation formula](../../../../../barycentric-interpolation-formula.md)

$$
\boxed{p_n(x)=
\frac{\displaystyle\sum_{s=0}^nw_su_s/(x-x_s)}
{\displaystyle\sum_{s=0}^nw_s/(x-x_s)}.}
$$

At $x=x_r$, use the continuous limiting value $u_r$. Multiplying every weight by the same nonzero constant cancels between numerator and denominator, so only relative weights are needed in computation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
