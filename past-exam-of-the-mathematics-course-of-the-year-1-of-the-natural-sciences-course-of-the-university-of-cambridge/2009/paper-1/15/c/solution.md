<h1 id="15/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At an intersection, $a+tu=b+t'v$, so $b-a=tu-t'v$. Alternating multilinearity of the [scalar triple product](../../../../../scalar-triple-product.md) then gives $[v,b-a,u]=t[v,u,u]-t'[v,v,u]=0$, establishing $[v,b,u]=[v,a,u]$.

For the location, write $b=a+tu-t'v$ and take its [scalar triple product](../../../../../scalar-triple-product.md) with $a$ and $v$:

$$
[a,b,v]=[a,a+tu-t'v,v]=t[a,u,v].
$$

Under the additional stated assumption $[a,u,v]\ne0$, division gives

$$
\boxed{r=a+\frac{[a,b,v]}{[a,u,v]}u.}
$$

These are [intersection parameters from scalar triple products](../../../../../intersection-parameters-from-scalar-triple-products.md). The formula presupposes an intersection; the first coplanarity condition by itself also holds for distinct parallel lines. Intersections can exist with the displayed denominator zero, in which case a different auxiliary vector or a component calculation is needed.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
