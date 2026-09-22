<h1 id="17b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes.** The Euler recurrence is

$$
y_{n+1}=y_n-h\operatorname{sign}(y_n).
$$

Write $y_0=mh+r$, where $m=\lfloor y_0/h\rfloor$ and $0\leq r<h$. For $n\leq m$, the numerical values agree with the exact linear descent. If $r=0$, the method reaches zero and stays there. If $0<r<h$, then

$$
y_m=r,\qquad y_{m+1}=r-h,
$$

and the recurrence thereafter alternates between $r$ and $r-h$. The exact solution is then zero, while both numerical values have magnitude at most $h$. Thus, uniformly for $0\leq n\leq N$,

$$
|y_n-y(nh)|\leq h=O(h).
$$

This is the [explicit Euler method for the sign-decay equation](../../../../../../explicit-euler-method-for-the-sign-decay-equation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17B](../../17b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
