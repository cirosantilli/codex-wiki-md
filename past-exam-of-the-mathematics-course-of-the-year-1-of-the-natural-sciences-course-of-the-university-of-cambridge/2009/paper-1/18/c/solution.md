<h1 id="18/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a=f(b,c)$ and work where both $f_b$ and $f_c$ are nonzero, so the required inverse [partial derivatives](../../../../../partial-derivative.md) exist. At fixed $a$, the [total differential](../../../../../total-differential.md) gives $0=f_b\,db+f_c\,dc$, hence $(\partial b/\partial c)_a=-f_c/f_b$. At fixed $b$, $(\partial c/\partial a)_b=1/f_c$. Their product with $f_b$ is $-1$: this is the [cyclic partial derivative identity](../../../../../cyclic-partial-derivative-identity.md).

For explicit verification in this example, put $P=b^4-6b^2c^2+c^4$ and $H=(b^2+c^2)^3$. Direct [differentiation](../../../../../differentiation.md) gives

$$
\left(\frac{\partial a}{\partial b}\right)_c=-\frac{cP}{H},\quad
\left(\frac{\partial a}{\partial c}\right)_b=\frac{bP}{H},\quad
\left(\frac{\partial b}{\partial c}\right)_a=\frac bc,\quad
\left(\frac{\partial c}{\partial a}\right)_b=\frac H{bP}.
$$

Therefore

$$
\boxed{\left(\frac{\partial a}{\partial b}\right)_c\left(\frac{\partial b}{\partial c}\right)_a\left(\frac{\partial c}{\partial a}\right)_b=-1.}
$$

The identity is local to regular branches: for these explicit formulas require $bcP\ne0$. At singular points one cannot justify cancellation of nonexistent inverse derivatives merely by writing a formal product.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [18](../../18.md)
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
