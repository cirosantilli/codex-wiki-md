<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [base case](../../../../../../base-case.md) $n=3$ is

$$
\frac1{3(3-2)}=\frac13=\frac34-\frac5{12}.
$$

Assume the displayed formula holds at some $n\geq3$. Adding the next term yields

$$
\begin{aligned}
\sum_{i=3}^{n+1}\frac1{i(i-2)}
&=\frac34-\frac{2n-1}{2n(n-1)}+\frac1{(n+1)(n-1)}\\
&=\frac34-\frac{(2n-1)(n+1)-2n}{2n(n-1)(n+1)}\\
&=\frac34-\frac{2n+1}{2n(n+1)}.
\end{aligned}
$$

The last step uses $(2n-1)(n+1)-2n=(2n+1)(n-1)$. This is the required formula at $n+1$, completing the proof by [mathematical induction](../../../../../../mathematical-induction.md). **The identity holds for all $n\geq3$.**

## ↑ Ancestors (13)

1. [I](../i.md)
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
