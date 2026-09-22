<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [method of undetermined coefficients](../../../../method-of-undetermined-coefficients.md) with the [polynomial](../../../../polynomial-split.md) $f_p=at^3+bt^2+ct+d$. Substitution into $f_p''+3f_p'+2f_p$ gives

$$
2at^3+(9a+2b)t^2+(6a+6b+2c)t+(2b+3c+2d).
$$

Matching successive coefficients with the forcing gives $a=1$, $b=-3$, $c=4$ and $d=1$. Hence a [particular integral](../../../../particular-solution.md) is

$$
\boxed{f_p(t)=t^3-3t^2+4t+1.}
$$

Indeed $f_p'=3t^2-6t+4$ and $f_p''=6t-6$ give $f_p''+3f_p'+2f_p=2t^3+3t^2-4t+8$. The [complementary function](../../../../homogeneous-solution.md), if wanted, is $C_1e^{-t}+C_2e^{-2t}$.

## ↑ Ancestors (12)

1. [B](../b.md)
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
