<h1 id="d/d3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $H_0=\int_0^\pi|h(u)|\,du<\infty$. On each period, substitute $x=j\pi+u$ and use periodicity:

$$
\int_{j\pi}^{(j+1)\pi}e^{-\beta x}|h(x)|\,dx
=e^{-\beta j\pi}\int_0^\pi e^{-\beta u}|h(u)|\,du
\leq e^{-\beta j\pi}H_0.
$$

Summing over $j\geq0$ gives the convergent geometric bound

$$
\boxed{\int_0^\infty e^{-\beta x}|h(x)|\,dx\leq\frac{H_0}{1-e^{-\beta\pi}}<\infty.}
$$

Measurability is preserved under multiplication by the exponential, so this proves [Lebesgue integrability](../../../../../../integrability.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [D3](../../../d3.md)
4. [D](../../../../d.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
