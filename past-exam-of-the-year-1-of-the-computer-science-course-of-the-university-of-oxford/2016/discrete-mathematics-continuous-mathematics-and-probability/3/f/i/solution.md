<h1 id="3/f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Prove the explicit bound $n!\leq2^{n^2}$ by [mathematical induction](../../../../../../mathematical-induction.md). At $n=1$, $1\leq2$. For the step, note that $n+1\leq2^n$ for $n\geq1$: this auxiliary inequality has base $2=2$ and follows at the next index from $n+2\leq2(n+1)$. Hence, using the [induction hypothesis](../../../../../../induction-hypothesis.md),

$$
(n+1)!\leq(n+1)2^{n^2}\leq2^{n^2+n}\leq2^{(n+1)^2}.
$$

Thus **$n!=O((2^n)^n)$**, with constant $1$ and threshold $1$ in [big O notation](../../../../../../big-o-notation.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [F](../../f.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
