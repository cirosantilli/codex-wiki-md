<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take

$$
f_1(n)=2n,\quad g_1(n)=n,\quad f_2(n)=g_2(n)=2^n.
$$

The premises hold with constants two and one. But

$$
\frac{f_2(f_1(n))}{g_2(g_1(n))}=\frac{2^{2n}}{2^n}=2^n\longrightarrow\infty.
$$

No fixed bounding constant can satisfy the proposed conclusion. This proves the [failure of unrestricted Big O composition](../../../../../failure-of-unrestricted-big-o-composition.md): a constant factor in an inner argument can become an unbounded factor after applying an exponential.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
