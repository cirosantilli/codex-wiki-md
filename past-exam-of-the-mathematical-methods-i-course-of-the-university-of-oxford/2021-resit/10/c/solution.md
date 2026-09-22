<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [differential operator](../../../../differential-operator.md) is $(D-1)^2$, with $D=d/dt$. Because $e^t$ already occurs in the [complementary function](../../../../homogeneous-solution.md) with a repeated [root of a polynomial](../../../../root-of-a-polynomial.md), an unmodified trial $Ce^t$ gives zero. Put $f_p=e^t h(t)$. The [product rule](../../../../product-rule.md) yields

$$
(D-1)(e^th)=e^th',\qquad (D-1)^2(e^th)=e^th''.
$$

Thus $h''=2$, and we may choose $h=t^2$, giving

$$
\boxed{f_p(t)=t^2e^t.}
$$

The other terms arising on twice integrating $h''=2$ give $(C_1+C_2t)e^t$, exactly the [complementary function](../../../../homogeneous-solution.md), so they need not be included in the [particular integral](../../../../particular-solution.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
