<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The base case is $F_5=5$, so $5\mid F_5$. To relate successive blocks of five, use the [Fibonacci addition formula](../../../../../fibonacci-addition-formula.md):

$$
F_{k+5}=F_5F_{k+1}+F_4F_k=5F_{k+1}+3F_k.
$$

This identity can also be obtained simply by applying the [Fibonacci recurrence](../../../../../fibonacci-recurrence.md) five times. If the [mathematical induction](../../../../../mathematical-induction.md) hypothesis is $5\mid F_{5n}$, then

$$
F_{5(n+1)}=5F_{5n+1}+3F_{5n}
$$

is a sum of two multiples of five. Hence

$$
\boxed{F_5\mid F_{5n}\quad\text{for every integer }n>0.}
$$

The generalisation is [Fibonacci multiple-index divisibility](../../../../../fibonacci-multiple-index-divisibility.md):

$$
\boxed{F_m\mid F_{mn}\quad(m,n\geq1).}
$$

Indeed, $F_{mn+m}=F_mF_{mn+1}+F_{m-1}F_{mn}$, so precisely the same [mathematical induction](../../../../../mathematical-induction.md) works with $5$ replaced by $m$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
