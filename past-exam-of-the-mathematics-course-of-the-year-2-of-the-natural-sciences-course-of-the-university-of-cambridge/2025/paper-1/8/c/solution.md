<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the shifted variable $t=y-1$, substitute the [Frobenius solution](../../../../../frobenius-solution.md) $x=\sum_{j\geq0}a_jt^{j+\sigma}$ into $t(t+2)x''+x'+x=0$. Equating the coefficient of $t^{j+\sigma}$ gives

$$
(j+1+\sigma)[2(j+\sigma)+1]a_{j+1}+[(j+\sigma)(j+\sigma-1)+1]a_j=0.
$$

Thus the [linear recurrence relation](../../../../../linear-recurrence-relation.md), valid for $j=0,1,\ldots$, is

$$
\boxed{a_{j+1}=-\frac{(j+\sigma)(j+\sigma-1)+1}{(j+1+\sigma)[2(j+\sigma)+1]}a_j.}
$$

For the [indicial root](../../../../../indicial-root.md) $\sigma=0$, this becomes

$$
a_{j+1}=-\frac{j^2-j+1}{(j+1)(2j+1)}a_j,\qquad \boxed{a_1=-a_0}.
$$

For the [indicial root](../../../../../indicial-root.md) $\sigma=1/2$, rename the coefficients $b_j$; then

$$
b_{j+1}=-\frac{j^2+3/4}{(j+3/2)(2j+2)}b_j,\qquad \boxed{b_1=-\frac14b_0}.
$$

With $a_0=b_0=1$, the first terms of the two [Frobenius solutions](../../../../../frobenius-solution.md) are

$$
\boxed{x_1=1-t+\frac16t^2+O(t^3),\qquad x_2=t^{1/2}\left(1-\frac14t+\frac7{160}t^2+O(t^3)\right).}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
