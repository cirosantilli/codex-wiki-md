<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

The characteristic polynomial of the [linear recurrence relation](../../../../../linear-recurrence-relation.md) is

$$
r^3-6r^2+12r-8=(r-2)^3.
$$

The repeated-root rule therefore gives

$$
x_n=(A+Bn+Cn^2)2^n.
$$

The condition $x_0=0$ gives $A=0$. The other two conditions give

$$
2(B+C)=4,\qquad
4(2B+4C)=24,
$$

so $B+C=2$ and $B+2C=3$. Thus $B=C=1$, and

$$
\boxed{x_n=n(n+1)2^n}.
$$

## ↑ Ancestors (10)

1. [2B](../2b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
