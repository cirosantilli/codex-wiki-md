<h1 id="19/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The supplied bracket gives $0<e_0=1.5-\sqrt2<0.1$. Part (b) ensures $x_n>\sqrt2>1.4$, so each error satisfies

$$
0<e_{n+1}<\frac{e_n^2}{2.8}.
$$

Writing $d_n=e_n/2.8$ gives $d_{n+1}<d_n^2$ and $d_0<0.1/2.8=1/28$. After three steps the exponent has doubled three times:

$$
\boxed{0<e_3<\frac{2.8}{28^8}\approx7.4113\times10^{-12}<10^{-11}.}
$$

This rigorous [error bound](../../../../../error-bound.md) uses only the given bracket, not advance knowledge of the digits of $\sqrt2$.

The actual rational iterates are $x_1=17/12$, $x_2=577/408$, and $x_3=665857/470832\approx1.414213562374690$. They illustrate the bound, but the proof comes from the exact error identity and the positive lower bound on the denominators.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
