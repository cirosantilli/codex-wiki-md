<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The trigonometric addition formula gives

$$
\sin((n+1)\theta)+\sin((n-1)\theta)=2\cos\theta\sin(n\theta).
$$

Dividing by $\sin\theta$ and writing $x=\cos\theta$ gives the [recurrence relation](../../../../../recurrence-relation.md)

$$
\boxed{y_{n+1}=2xy_n-y_{n-1}.}
$$

The first two members are $y_1=1$ and $y_2=2x$. If $y_n$ has degree $n-1$ and leading coefficient $2^{n-1}$, then $2xy_n$ has degree $n$ and leading coefficient $2^n$, whereas $y_{n-1}$ has lower degree and cannot cancel that term. [Mathematical induction](../../../../../mathematical-induction.md) proves

$$
\boxed{\deg y_n=n-1,\qquad\text{leading coefficient of }y_n=2^{n-1}.}
$$

For example the sequence begins $1,2x,4x^2-1,8x^3-4x$, agreeing with the [Chebyshev polynomial of the second kind](../../../../../chebyshev-polynomial-of-the-second-kind.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
