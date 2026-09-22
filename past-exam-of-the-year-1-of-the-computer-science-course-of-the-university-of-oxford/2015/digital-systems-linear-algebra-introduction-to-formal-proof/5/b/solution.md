<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Both signs are positive, so perform [addition](../../../../../addition.md) of the aligned [significands](../../../../../significand.md). The true [exponents](../../../../../exponent.md) are $-1$ and $3$, a difference of four. Shift the smaller [significand](../../../../../significand.md) right four places, retaining its low [bits](../../../../../bit.md):

$$
\frac58=0.000101_2\,2^3,\qquad15\frac12=1.111100_2\,2^3.
$$

Add at the common [exponent](../../../../../exponent.md):

$$
\begin{array}{r}
1.111100_2\\
+\;0.000101_2\\\hline
10.000001_2
\end{array}
\qquad\text{so}\qquad10.000001_2\,2^3=1.0000001_2\,2^4.
$$

Renormalization raises the true [exponent](../../../../../exponent.md) to $4$ and the biased [exponent](../../../../../exponent.md) to $E=19=10011_2$. There are only seven fraction places to retain, so no [floating-point rounding](../../../../../floating-point-rounding.md) changes the result:

$$
\boxed{\frac58+15\frac12=16\frac18,\qquad\text{stored fields }0\;10011\;0000001000.}
$$

The complete word is `0100110000001000`.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
