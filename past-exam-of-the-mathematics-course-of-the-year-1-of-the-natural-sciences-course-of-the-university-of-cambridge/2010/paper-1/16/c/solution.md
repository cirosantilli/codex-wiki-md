<h1 id="16/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $B(n,n)=\int_0^1[x(1-x)]^{n-1}dx$ and set $v=2x-1$. Since $x(1-x)=(1-v^2)/4$ and $dx=dv/2$,

$$
B(n,n)=2^{1-2n}\int_{-1}^{1}(1-v^2)^{n-1}dv
=2^{2-2n}\int_0^1(1-v^2)^{n-1}dv.
$$

In the last integral put $u=v^2$, giving $dv=du/(2\sqrt u)$. This yields $B(n,n)=2^{1-2n}B(1/2,n)$, and part (a) interchanges the arguments. Hence

$$
\boxed{B(n,n)=\frac{B(n,1/2)}{2^{2n-1}}.}
$$

The [equal-argument beta integral](../../../../../equal-argument-beta-integral.md) identity holds for every positive real $n$, not only positive integers.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [16](../../16.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
