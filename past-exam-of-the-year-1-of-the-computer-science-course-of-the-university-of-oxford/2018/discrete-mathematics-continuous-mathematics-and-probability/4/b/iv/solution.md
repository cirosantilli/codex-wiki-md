<h1 id="4/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Seek a periodic [particular solution](../../../../../../particular-solution.md) with [Fourier coefficients](../../../../../../fourier-coefficient.md) $A_n,B_n$. Comparing constant terms gives $A_0=a_0/2$. Comparing the cosine and sine terms for $n\geq1$ gives

$$
2A_n+nB_n=a_n,\qquad -nA_n+2B_n=0,
$$

so $A_n=2a_n/(n^2+4)$ and $B_n=na_n/(n^2+4)$. Insert the coefficients from part (a) and add the [homogeneous solution](../../../../../../homogeneous-solution.md):

$$
\boxed{y(x)=Ce^{-2x}+\frac1\pi-\frac2\pi\sum_{m=1}^\infty\frac{\cos(2mx)+m\sin(2mx)}{(4m^2-1)(m^2+1)}.}
$$

The differentiated series converges absolutely and uniformly, because its largest coefficient terms are $O(m^{-2})$. This justifies the term-by-term first [derivative](../../../../../../derivative.md) used in substituting into the [differential equation](../../../../../../differential-equation-split.md). Any two solutions differ by $Ce^{-2x}$, proving that the displayed family is the general solution. The computation is an instance of [Fourier response of a first-order linear differential equation](../../../../../../fourier-response-of-a-first-order-linear-differential-equation.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
