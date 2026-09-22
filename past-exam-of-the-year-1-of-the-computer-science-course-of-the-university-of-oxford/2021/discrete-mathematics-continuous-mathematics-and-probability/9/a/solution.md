<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Condition on the fair coin choosing the initial chamber. The [law of total probability](../../../../../law-of-total-probability.md) gives $\mathbb P(\text{reach }k)=(p_1+p_2)/2$. With $r=(1-p)/p$, substituting the [biased gambler's ruin probability](../../../../../biased-gambler-s-ruin-probability.md) gives

$$
\boxed{\mathbb P(\text{reach }k)=
\begin{cases}
\displaystyle\frac{2-r-r^2}{2(1-r^k)},&p\ne\tfrac12,\\[5pt]
\displaystyle\frac3{2k},&p=\tfrac12.
\end{cases}}
$$

Both numerator and denominator in the first case have the same sign. Its limit as $r\to1$ is the fair-walk value, since the ratio of their first [derivatives](../../../../../derivative.md) is $3/(2k)$. The averaging is over initial locations, not over the transition [probabilities](../../../../../probability.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
