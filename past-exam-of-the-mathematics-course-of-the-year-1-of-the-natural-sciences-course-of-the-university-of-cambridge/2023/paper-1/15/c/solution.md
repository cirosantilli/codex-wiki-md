<h1 id="15/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Factor the leading term out of the [Maclaurin series](../../../../../maclaurin-series.md) for the [sine](../../../../../sine.md):

$$
\sin x=x\left(1-\frac{x^2}{6}+\frac{x^4}{120}+O(x^6)\right).
$$

The [binomial theorem](../../../../../binomial-theorem.md) gives, through degree four inside the bracket,

$$
\left(1-\frac{x^2}{6}+\frac{x^4}{120}+O(x^6)\right)^6=1+6\left(-\frac{x^2}{6}+\frac{x^4}{120}\right)+\binom62\frac{x^4}{36}+O(x^6).
$$

The coefficient of $x^4$ is $1/20+5/12=7/15$. Multiplying back by $x^6$ yields

$$
\boxed{\sin^6x=x^6-x^8+\frac7{15}x^{10}+O(x^{12}).}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
