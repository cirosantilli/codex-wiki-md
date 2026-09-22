<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At $u_0=0$, the [linear-system residual](../../../../../../linear-system-residual.md) is $r_0=b=(1,1)^T$. Here $Ar_0=r_0$, so the [steepest-descent step size](../../../../../../steepest-descent-step-size.md) is

$$
\frac{r_0^Tr_0}{r_0^TAr_0}=\frac22=1.
$$

Consequently **$u_1=(1,1)^T$**, and $Au_1=b$ gives residual zero. The stated exact-arithmetic stopping test with $\epsilon=0$ is met after one iteration. Stop there rather than trying to evaluate the next, undefined $0/0$ step. This is the special case where the initial residual is an [eigenvector](../../../../../../eigenvector.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
