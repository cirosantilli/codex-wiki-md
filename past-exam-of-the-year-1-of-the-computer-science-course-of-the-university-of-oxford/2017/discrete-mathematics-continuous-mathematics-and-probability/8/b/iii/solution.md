<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The initial values are $p_0=1$ and $p_1=1/2$. The [characteristic polynomial](../../../../../../characteristic-polynomial.md) of the [linear recurrence](../../../../../../linear-recurrence-relation.md) is

$$
16r^2-8r-3=(4r-3)(4r+1),
$$

with roots $3/4$ and $-1/4$. Hence $p_n=a(3/4)^n+b(-1/4)^n$. The initial conditions give $a+b=1$, $3a-b=2$, so $a=3/4$, $b=1/4$. Therefore

$$
\boxed{p_n=\frac34\left(\frac34\right)^n+\frac14\left(-\frac14\right)^n
=\frac{3^{n+1}+(-1)^n}{4^{n+1}},\qquad n\geq0.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
