<h1 id="d/d3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The integrand is nonnegative and measurable. It is [bounded](../../../../../boundedness.md) by $x$ near zero and by $xe^{-x}$ for $x>0$, so its integral is finite. For every $x>0$ the geometric expansion gives $x/(e^x+1)=\sum_{n\ge1}(-1)^{n-1}xe^{-nx}$. To justify termwise integration, note that

$$
\sum_{n\ge1}\int_0^\infty|(-1)^{n-1}xe^{-nx}|dx=\sum_{n\ge1}\frac1{n^2}<\infty.
$$

Tonelli gives an [integrable](../../../../../integrability.md) sum of absolute values; [dominated convergence](../../../../../dominated-convergence-theorem.md) then applies to the signed partial sums. Consequently

$$
\boxed{\int_0^\infty\frac{x}{e^x+1}dx=\sum_{n\ge1}\frac{(-1)^{n-1}}{n^2}.}
$$

If evaluated further, this is $(1-2^{-1})\zeta(2)=\pi^2/12$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D3](../../d3.md)
3. [D](../../../d.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
