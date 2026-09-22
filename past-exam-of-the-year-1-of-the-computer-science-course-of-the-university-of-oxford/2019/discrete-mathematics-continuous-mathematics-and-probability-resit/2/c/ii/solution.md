<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [mathematical induction](../../../../../../mathematical-induction.md) with two consecutive [base cases](../../../../../../base-case.md): $F_2=1=(3/2)^0$ and $F_3=2\geq(3/2)^1$. Suppose the bounds hold for exponents $n$ and $n+1$. The [Fibonacci recurrence](../../../../../../fibonacci-recurrence.md) gives

$$
F_{n+4}=F_{n+3}+F_{n+2}\geq(3/2)^{n+1}+(3/2)^n=\frac52(3/2)^n\geq\frac94(3/2)^n=(3/2)^{n+2}.
$$

Thus the consecutive pair of bounds advances one step. **$F_{n+2}\geq(3/2)^n$ for every $n\geq0$.**

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
