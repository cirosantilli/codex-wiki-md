<h1 id="d/d4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $x=e^{-t}$. Then

$$
\int_0^1(x\log x)^k\,dx
=(-1)^k\int_0^\infty t^k e^{-(k+1)t}\,dt
=\boxed{\frac{(-1)^k k!}{(k+1)^{k+1}}},
$$

where the second substitution is $u=(k+1)t$ and the final [integral](../../../../../integral-split.md) is the given [gamma function](../../../../../gamma-function.md) value. The formula also holds for $k=0$, with value $1$.

For $0<x<1$, the [exponential function](../../../../../exponential-function.md) expansion gives

$$
x^{-x}=e^{-x\log x}=\sum_{k=0}^\infty\frac{(-x\log x)^k}{k!}.
$$

Every term is nonnegative. By the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md), integration can be interchanged with summation, and hence

$$
\int_0^1x^{-x}\,dx
=\sum_{k=0}^\infty\frac1{(k+1)^{k+1}}
=\boxed{\sum_{j=1}^\infty\frac1{j^j}}.
$$

This identity is one form of [Sophomore's dream](../../../../../sophomore-s-dream.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [D4](../../d4.md)
3. [D](../../../d.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
