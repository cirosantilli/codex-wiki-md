<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $n=1$, both sides are $1/3$. Assuming the formula through $n$, adding the next term gives

$$
\begin{aligned}
\sum_{i=1}^{n+1}\frac1{(2i-1)(2i+1)}
&=\frac{n}{2n+1}+\frac1{(2n+1)(2n+3)}\\
&=\frac{2n^2+3n+1}{(2n+1)(2n+3)}
=\frac{n+1}{2n+3}.
\end{aligned}
$$

The last expression is the required formula at $n+1$, completing [mathematical induction](../../../../../../mathematical-induction.md). The [partial fraction decomposition](../../../../../../partial-fraction-decomposition.md)

$$
\frac1{(2i-1)(2i+1)}=\frac12\left(\frac1{2i-1}-\frac1{2i+1}\right)
$$

provides a second explanation: this is a [telescoping sum](../../../../../../telescoping-sum.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
