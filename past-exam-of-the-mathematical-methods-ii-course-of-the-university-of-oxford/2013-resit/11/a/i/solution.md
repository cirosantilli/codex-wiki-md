<h1 id="11/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a twice continuously differentiable function, a finite second-order [Taylor expansion](../../../../../taylor-expansion.md) about an interior point is

$$
f(x+a,y+b)=f(x,y)+f_xa+f_yb+\frac12(Aa^2+2Bab+Cb^2)+o(a^2+b^2),
$$

where $A=f_{xx}$, $B=f_{xy}$, $C=f_{yy}$ at that point. A differentiable interior extremum requires $f_x=f_y=0$. For a strict minimum guaranteed by the quadratic term, the [Hessian matrix](../../../../../hessian-matrix.md) must be positive definite. Completing the square gives $Aa^2+2Bab+Cb^2=A(a+Bb/A)^2+(AC-B^2)b^2/A$. Thus sufficient nondegenerate minimum conditions are

$$
\boxed{f_x=f_y=0,\qquad A>0,\qquad D=AC-B^2>0.}
$$

If $D=0$, the second-order test is inconclusive; for example $x^4+y^4$ has a strict minimum at zero despite a zero Hessian. The finite Taylor argument only needs $C^2$ regularity. The source's infinite Taylor representation additionally needs suitable analyticity: a smooth [flat function](../../../../../flat-function.md), such as $e^{-1/(x^2+y^2)}$ extended by zero at the origin, has every Taylor coefficient zero there but is positive nearby.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [11](../../../11.md)
4. [2013 resit](../../../../2013-resit-split.md)
5. [Past exam of the mathematical methods II course of the University of Oxford](../../../../split.md)
6. [Mathematical methods II course of the University of Oxford](../../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
