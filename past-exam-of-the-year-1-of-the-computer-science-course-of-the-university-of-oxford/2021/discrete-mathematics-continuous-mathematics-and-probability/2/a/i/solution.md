<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the base case $n=2$, the product is $1-1/4=3/4=(2+1)/(2\cdot2)$. Assume the identity holds for some $n\geq2$. Multiplying by the next factor gives

$$
\begin{aligned}
\prod_{i=2}^{n+1}\left(1-\frac1{i^2}\right)
&=\frac{n+1}{2n}\left(1-\frac1{(n+1)^2}\right)\\
&=\frac{n+1}{2n}\frac{n(n+2)}{(n+1)^2}
=\frac{n+2}{2(n+1)}.
\end{aligned}
$$

This is the desired expression with $n$ replaced by $n+1$, so [mathematical induction](../../../../../../mathematical-induction.md) proves the identity for every $n\geq2$. The factorization $1-i^{-2}=(i-1)(i+1)/i^2$ also explains the cancellation as a [telescoping product](../../../../../../telescoping-product.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
