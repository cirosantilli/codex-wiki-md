<h1 id="b/4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For any vectors $a,b$,

$$
|a^Tb|\leq\sum_j|a_j||b_j|\leq\|a\|_\infty\sum_j|b_j|=\boxed{\|a\|_\infty\|b\|_1}.
$$

Thus, among directions with $\|d\|_\infty\leq1$, $g^Td\geq-\|g\|_1$. Equality is achieved by

$$
\boxed{d_j=-\operatorname{sgn}(g_j)\quad(g_j\ne0),\qquad d_j\in[-1,1]\quad(g_j=0).}
$$

For $g\ne0$ these minimizing directions have infinity norm one. The strongest decrease per unit infinity-norm step is $-\|g\|_1$, illustrating the [dual norm](../../../../../dual-norm.md) pairing between the infinity norm and the one-norm.

To match the unnormalized convention in part (a), minimize $g^Ts+\tfrac12\|s\|_\infty^2$. At fixed $t=\|s\|_\infty$, its minimum is $-t\|g\|_1+\tfrac12t^2$, attained at $t=\|g\|_1$. One conventional choice is therefore $\boxed{s=-\|g\|_1\operatorname{sgn}(g)}$, with zero entries where $g_j=0$. Its ray agrees with the unit direction just computed.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
