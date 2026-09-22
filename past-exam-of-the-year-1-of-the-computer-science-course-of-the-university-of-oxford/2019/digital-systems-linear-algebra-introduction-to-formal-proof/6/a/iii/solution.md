<h1 id="6/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [spectral error bound for a diagonalizable fixed-point iteration](../../../../../../spectral-error-bound-for-a-diagonalizable-fixed-point-iteration.md), the exact solution $x$ is a [fixed point](../../../../../../fixed-point.md): $x=Gx+c$. Subtracting it from the iteration gives the error recurrence $e_n=Ge_{n-1}$, with $e_n=x_n-x$. Multiplying by $S^{-1}$ and using $G=SDS^{-1}$ gives

$$
f_n=S^{-1}GSf_{n-1}=Df_{n-1}.
$$

Iterating proves **$f_n=D^nf_0$**, including $n=0$ because $D^0=I$. This argument does not assume $S$ is [orthogonal](../../../../../../orthogonal-vectors.md); it simply expresses the error in an [eigenbasis](../../../../../../eigenbasis.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
