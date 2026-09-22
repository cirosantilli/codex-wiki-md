<h1 id="10/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the exact difference, the representability condition becomes

$$
\boxed{-H\leq x-y\leq U\quad\Longleftrightarrow\quad x-U\leq y\leq x+H.}
$$

Within the same operand square $[-H,U]^2$, the closed diagonal band between $y=x-U$ and $y=x+H$ is representable. Above the upper line, $x-y<-H$ gives negative overflow; below the lower line, $x-y>U$ gives positive overflow. The right-hand panel of the figure shows these regions, including their representable boundary points.

Positive overflow can occur only when $x\geq0$ and $y<0$; negative overflow can occur only when $x<0$ and $y\geq0$. The corresponding exact inequalities are still required: operands with different signs do not always overflow. Same-sign subtraction is always representable. In sign-[bit](../../../../../../bit.md) terms, subtraction overflows exactly when the operands have different signs and the wrapped result's sign differs from that of $x$.

One must test subtraction directly or use its correct overflow rule: forming `-y` in the same $n$ [bits](../../../../../../bit.md) fails at $y=-H$, even though some differences with that operand are representable. For example $(-H)-(-H)=0$ is valid.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [10](../../../10.md)
4. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
