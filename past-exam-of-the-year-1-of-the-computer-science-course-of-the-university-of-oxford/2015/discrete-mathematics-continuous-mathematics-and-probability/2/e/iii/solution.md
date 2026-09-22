<h1 id="2/e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use [mathematical induction](../../../../../../mathematical-induction.md) with two base cases. At $n=0$, the formula gives $(1-1)/\sqrt5=0=F_0$. At $n=1$, it gives $(\phi-\psi)/\sqrt5=1=F_1$.

If it holds at $n-1$ and $n$, then the [Fibonacci recurrence](../../../../../../fibonacci-recurrence.md) gives

$$
F_{n+1}=\frac{\phi^n+\phi^{n-1}-\psi^n-\psi^{n-1}}{\sqrt5}.
$$

The identities $\phi^2=\phi+1$ and $\psi^2=\psi+1$ turn the numerator into $\phi^{n+1}-\psi^{n+1}$. Thus

$$
\boxed{F_n=(\phi^n-\psi^n)/\sqrt5\quad\text{for every }n\ge0.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [E](../../e.md)
3. [2](../../../2.md)
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
