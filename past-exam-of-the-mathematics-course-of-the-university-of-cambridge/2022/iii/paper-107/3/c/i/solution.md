<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Taylor's theorem and $g(0)=g'(0)=0$ give

$$
|g(s)|\leq\frac12|s|^2,
\qquad
|g'(s)|\leq|s|
\quad(|s|\leq1).
$$

Combining these with the product estimate in a [Hölder space](../../../../../../../holder-space.md) yields

$$
\boxed{|g(u)|_{0,\alpha;B}\leq|u|_{0,\alpha;B}^2.}
$$

Writing

$$
g(u_1)-g(u_2)=(u_1-u_2)
\int_0^1g'(u_2+t(u_1-u_2))\,dt
$$

and using the same product estimate gives

$$
\boxed{|g(u_1)-g(u_2)|_{0,\alpha;B}
\leq(|u_1|_{0,\alpha;B}+|u_2|_{0,\alpha;B})
|u_1-u_2|_{0,\alpha;B}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
