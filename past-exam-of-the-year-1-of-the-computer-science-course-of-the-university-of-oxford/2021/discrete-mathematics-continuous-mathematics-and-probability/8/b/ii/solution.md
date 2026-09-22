<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Compute all three [probabilities](../../../../../../probability.md). From the preceding part, $\mathbb P(A)=e^{-6}$. Integrating the [joint probability density function](../../../../../../joint-probability-density.md) over $u>v$ gives

$$
\mathbb P(B)=\int_0^\infty\int_v^\infty2e^{-u-2v}\,du\,dv
=\int_0^\infty2e^{-3v}\,dv=\frac23.
$$

On $A\cap B$ one has $v>2$ and $u>v$, so

$$
\mathbb P(A\cap B)=\int_2^\infty\int_v^\infty2e^{-u-2v}\,du\,dv
=\frac23e^{-6}=\mathbb P(A)\mathbb P(B).
$$

Therefore **$A$ and $B$ are independent events**. The minimum waiting time and the identity of the first clock are independent for [competing exponential clocks](../../../../../../competing-exponential-clocks.md); unequal rates change the winner [probabilities](../../../../../../probability.md) but do not destroy that [independence](../../../../../../independent-random-variables.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
