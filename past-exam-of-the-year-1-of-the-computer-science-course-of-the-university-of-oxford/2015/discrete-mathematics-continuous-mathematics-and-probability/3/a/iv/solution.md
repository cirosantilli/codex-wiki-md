<h1 id="3/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A direct [mathematical induction](../../../../../../mathematical-induction.md) proves $0\le F_n\le2^n$. The base cases $F_0=0\le1$ and $F_1=1\le2$ hold. If the bound holds at $n-1$ and $n$, then the [Fibonacci recurrence](../../../../../../fibonacci-recurrence.md) gives

$$
F_{n+1}=F_n+F_{n-1}\le2^n+2^{n-1}\le2^{n+1}.
$$

Thus the definition of [big O notation](../../../../../../big-o-notation.md) holds with $C=1$, proving

$$
\boxed{F_n=O(2^n).}
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
