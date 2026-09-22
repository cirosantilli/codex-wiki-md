<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $n\geq2$, $X_2+\cdots+X_n$ is independent of $X_1$ and has a [Poisson distribution](../../../../../../poisson-distribution.md) with parameter $(n-1)\lambda$. Part (ii) therefore gives

$$
X_1\mid(X_1+\cdots+X_n=n)\sim\operatorname{Bin}(n,1/n).
$$

Its probability at zero is

$$
\boxed{\mathbb P(X_1=0\mid X_1+\cdots+X_n=n)=\left(1-\frac1n\right)^n\quad(n\geq1)}.
$$

For $n=1$ the event being conditioned on is $X_1=1$, so the answer is $0$, also matching the displayed expression. The cancellation of $\lambda$ reflects the equal rates of all $n$ counts, not an approximation or large-$n$ limit.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
