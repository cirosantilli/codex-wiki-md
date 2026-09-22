<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Normalize the free leading coefficient to $a_0=1$. The [linear recurrence relation](../../../../../linear-recurrence-relation.md) from part (b) gives

$$
4a_2+4a_0=0,\qquad16a_4+2a_0=0,\qquad36a_6+12a_4=0.
$$

Consequently the first four nonzero coefficients are

$$
\boxed{a_0=1,\qquad a_2=-1,\qquad a_4=-\frac18,\qquad a_6=\frac1{24},}
$$

and the single pure [Frobenius solution](../../../../../frobenius-solution.md) is

$$
\boxed{y_1(z)=\frac1z\left(1-z^2-\frac18z^4+\frac1{24}z^6+O(z^8)\right).}
$$

For clarity about the second independent solution, a choice with no added multiple of $y_1$ is

$$
y_2=y_1\log z+\frac52z+\frac38z^3-\frac{11}{144}z^5+\frac{131}{9216}z^7+O(z^9).
$$

These companion coefficients follow by [reduction of order](../../../../../reduction-of-order.md) with the normalized [Wronskian](../../../../../wronskian.md) $W=z^{-3}(1+z^2)^{3/2}\exp[3z^2/(2(1+z^2))]$. The logarithm requires a local branch; it does not supply a second ordinary [power series](../../../../../power-series.md) solution.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
