<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $m\ge1$ and use two-base [mathematical induction](../../../../../mathematical-induction.md) on $n$. At $n=0$, the proposed right side is $F_m$; at $n=1$, it is $F_{m-1}+F_m=F_{m+1}$. Suppose the identity holds at $n$ and $n+1$. The defining [recurrence relation](../../../../../recurrence-relation.md) for the [Fibonacci numbers](../../../../../fibonacci-number.md) gives

$$
F_{m+n+2}=F_{m+n+1}+F_{m+n}
=F_{m-1}(F_{n+1}+F_n)+F_m(F_{n+2}+F_{n+1})
=F_{m-1}F_{n+2}+F_mF_{n+3}.
$$

This is the assertion at $n+2$, completing the proof of the [Fibonacci addition formula](../../../../../fibonacci-addition-formula.md). The argument includes $m=1$, since $F_{m-1}=F_0$ is defined.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
