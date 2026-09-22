<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substitute a smooth exact solution into the [linear multistep method](../../../../../linear-multistep-method-split.md) and expand about $x_n$. Its residual is

$$
(1+a+b)y+h(3+a-1)y'+h^2(9/2+a/2-2)y''+O(h^3).
$$

[Consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) requires the coefficients of $y$ and $hy'$ to vanish. Therefore $1+a+b=0$ and $3+a=1$, giving the unique choice

$$
\boxed{a=-2,\qquad b=1.}
$$

For this choice the next coefficient is $9/2-1-2=3/2\ne0$, so the residual is $\tfrac32h^2y''+O(h^3)$. The normalized [local truncation error](../../../../../local-truncation-error.md), obtained by dividing the residual by $h$, is $O(h)$. Hence **the method has order one**.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
