<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $s>t$, the coefficient bound gives $A(s)-A(t)\geq C_1(s-t)$. Thus for $0\leq s\leq t$ the positive kernel satisfies

$$
K(t,s):=e^{-(A(t)-A(s))}\leq e^{-C_1(t-s)},\qquad
\int_0^t K(t,s)\,ds\leq\frac{1-e^{-C_1t}}{C_1}\leq\frac1{C_1}.
$$

The starting [Picard iterate](../../../../../picard-iterate.md) is continuous and has [supremum norm](../../../../../supremum-norm.md) $M_0=|b|$. If the $n$th [Picard iterate](../../../../../picard-iterate.md) is bounded and continuous, its integral defines another [continuous function](../../../../../continuous-function.md), and

$$
|y_{n+1}(t)|\leq |b|e^{-A(t)}+M_n^2\int_0^tK(t,s)\,ds
\leq |b|+\frac{M_n^2}{C_1}.
$$

Taking the [supremum norm](../../../../../supremum-norm.md) and applying [mathematical induction](../../../../../mathematical-induction.md) proves boundedness of every iterate and

$$
\boxed{M_{n+1}\leq |b|+C_1^{-1}M_n^2.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
