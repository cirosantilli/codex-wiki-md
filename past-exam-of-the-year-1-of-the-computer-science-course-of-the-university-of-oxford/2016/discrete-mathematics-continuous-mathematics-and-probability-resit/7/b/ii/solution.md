<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $J$ count successful journeys before the first breakdown. The probability of surviving the first $r$ journeys is the [tail probability](../../../../../../tail-probability.md) $\mathbb P(J\geq r)$. For $d\geq0$, [independence](../../../../../../independent-random-variables.md) gives

$$
\mathbb P(J\geq2d+1)=q^d(1-\alpha),\qquad
\mathbb P(J\geq2d+2)=q^{d+1},
$$

where again $q=(1-\alpha)(1-\beta)$. For a nonnegative integer-valued [random variable](../../../../../../random-variable-split.md), the [tail-sum formula](../../../../../../tail-sum-formula.md) follows by writing $J=\sum_{r\geq1}\mathbf1_{\{J\geq r\}}$ and interchanging nonnegative sums. Therefore

$$
\begin{aligned}
\mathbb E(J)
&=\sum_{d=0}^{\infty}\left(q^d(1-\alpha)+q^{d+1}\right)\\
&=\boxed{\frac{(1-\alpha)+q}{1-q}=\frac{(1-\alpha)(2-\beta)}{\alpha+\beta-\alpha\beta}}.
\end{aligned}
$$

As a separate first-day check using the [law of total expectation](../../../../../../law-of-total-expectation.md), if $E=\mathbb E(J)$, then $E=\alpha\cdot0+(1-\alpha)\beta\cdot1+q(2+E)$. Solving gives the same finite value. This counts only successful journeys, excluding the failed journey.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
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
