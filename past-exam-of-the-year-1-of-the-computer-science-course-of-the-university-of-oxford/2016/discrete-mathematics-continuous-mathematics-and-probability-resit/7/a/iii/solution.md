<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [conditional expectation](../../../../../../conditional-expectation.md) given an event of positive probability is

$$
\boxed{\mathbb E(X\mid B_i)=\sum_{j=0}^{\infty}j\,\mathbb P(X=j\mid B_i)}.
$$

Apply the [law of total probability](../../../../../../law-of-total-probability.md) to each event $\{X=j\}$:

$$
\begin{aligned}
\mathbb E(X)
&=\sum_{j=0}^{\infty}j\sum_{i=1}^{k}\mathbb P(X=j\mid B_i)\mathbb P(B_i)\\
&=\sum_{i=1}^{k}\mathbb P(B_i)\sum_{j=0}^{\infty}j\,\mathbb P(X=j\mid B_i)\\
&=\boxed{\sum_{i=1}^{k}\mathbb P(B_i)\mathbb E(X\mid B_i)}.
\end{aligned}
$$

This is the [law of total expectation](../../../../../../law-of-total-expectation.md). Interchanging the sums is justified by nonnegative terms, for example by [Tonelli theorem](../../../../../../tonelli-theorem.md), so it remains valid when the expectation is infinite.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
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
