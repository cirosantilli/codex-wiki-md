<h1 id="g/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $I[y]=\int_a^bG(x,y,y')\,dx$. For endpoint-zero variations $\eta$, the [first variations](../../../../../first-variation.md) are

$$
\delta J(\eta)=\int_a^b(F_y\eta+F_{y'}\eta')\,dx,\qquad
\delta I(\eta)=\int_a^b(G_y\eta+G_{y'}\eta')\,dx.
$$

For a normal constrained [extremal](../../../../../extremal.md), choose a variation $\eta_0$ with $\delta I(\eta_0)\ne0$. Given any $\eta$, use the [implicit function theorem](../../../../../implicit-function-theorem.md) to choose a small correction in the $\eta_0$ direction so that $y+t\eta+s(t)\eta_0$ preserves the constraint. Differentiating it and the stationarity condition at zero gives

$$
\delta J(\eta)=\lambda\delta I(\eta),\qquad
\lambda=\frac{\delta J(\eta_0)}{\delta I(\eta_0)}.
$$

Integrate the derivative-of-variation term by parts. Since the variations vanish at both endpoints, the [boundary term](../../../../../boundary-term.md) is zero. The [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) then gives

$$
\boxed{(F-\lambda G)_y-\frac d{dx}(F-\lambda G)_{y'}=0.}
$$

The regularity condition on the constraint is what permits the coefficient of $F$ to be normalized to 1. In a degenerate case, the general multiplier statement uses $\lambda_0F-\lambda_1G$ with the two coefficients not both zero; the source's displayed form is the normal case.

For a string described as a [function graph](../../../../../graph-of-a-function.md) $r(x)=(x,y(x))$, its arc-length element is $|r'(x)|\,dx=\sqrt{1+y'(x)^2}\,dx$. Inextensibility therefore gives

$$
\boxed{\int_0^{2a}\sqrt{1+y'^2}\,dx=l.}
$$

This also forces $l\ge2a$, with equality only for the straight [function graph](../../../../../graph-of-a-function.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [G](../../../g.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
