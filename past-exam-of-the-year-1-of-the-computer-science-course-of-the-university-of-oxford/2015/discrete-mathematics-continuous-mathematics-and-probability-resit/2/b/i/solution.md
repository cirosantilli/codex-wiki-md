<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [mathematical induction](../../../../../../mathematical-induction.md). For $n=1$, the left side is $2^0=1=2^1-1$. If the identity holds at $n$, then

$$
\sum_{k=0}^{n}2^k
=\left(\sum_{k=0}^{n-1}2^k\right)+2^n
=(2^n-1)+2^n
=2^{n+1}-1.
$$

The base case and induction step establish the [geometric series](../../../../../../geometric-series.md) identity

$$
\boxed{\sum_{k=0}^{n-1}2^k=2^n-1\quad(n\geq1).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
