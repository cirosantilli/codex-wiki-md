<h1 id="p/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For any $q\in\Pi_n$, the difference $p-q$ lies in $\Pi_n$ and is orthogonal to $f-p$. The [Pythagorean theorem for inner product spaces](../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|f-q\|^2=\|(f-p)+(p-q)\|^2=\|f-p\|^2+\|p-q\|^2\geq\|f-p\|^2.
$$

Thus the [orthogonality](../../../../orthogonal-vectors.md) condition proves minimality, and equality forces $q=p$.

Write the requested linear [polynomial](../../../../polynomial-split.md) as $p=a+bx$. Orthogonality to one and $x$ gives

$$
\int_{-1}^1x^2(x^2-a-bx)dx=0,\qquad
\int_{-1}^1x^3(x^2-a-bx)dx=0.
$$

Odd integrals vanish, leaving $2/5-2a/3=0$ and $-2b/5=0$. Consequently

$$
\boxed{p(x)=3/5.}
$$

The weight's single zero does not destroy positive definiteness on continuous functions: a nonzero continuous function is nonzero on an interval containing points where $x^2>0$. The preceding projection argument therefore applies to this [inner product](../../../../inner-product-split.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [P](../../p.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
