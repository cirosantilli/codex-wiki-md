<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There is no forbidden pair in a [sequence](../../../../../../sequence.md) of length zero or one, so $p_0=p_1=1$. For $n\geqslant2$, divide acceptable [sequences](../../../../../../sequence.md) into two disjoint cases. If the first digit differs from $3$, its [probability](../../../../../../probability.md) is $2/3$, and the remaining $n-1$ independent digits must avoid the pair. If the first digit is $3$, the next must differ from $3$, which has combined [probability](../../../../../../probability.md) $2/9$, and the remaining $n-2$ digits must avoid the pair. The boundary between this prefix and the remaining digits cannot create a forbidden pair, because the prefix ends in a digit other than $3$. Consequently

$$
\boxed{p_n=\frac23p_{n-1}+\frac29p_{n-2},\qquad p_0=p_1=1.}
$$

The [characteristic polynomial of a linear recurrence](../../../../../../characteristic-polynomial-of-a-linear-recurrence.md) is $r^2-\frac23r-\frac29$, with distinct roots

$$
r_+=\frac{1+\sqrt3}{3},\qquad r_-=\frac{1-\sqrt3}{3}.
$$

Writing $p_n=Ar_+^n+Br_-^n$, the [initial conditions](../../../../../../initial-condition.md) give $A+B=1$ and $Ar_++Br_-=1$. Therefore

$$
\boxed{p_n=\frac{2+\sqrt3}{2\sqrt3}\left(\frac{1+\sqrt3}{3}\right)^n+\frac{\sqrt3-2}{2\sqrt3}\left(\frac{1-\sqrt3}{3}\right)^n,\qquad n\geqslant0.}
$$

For example, $p_2=8/9$, since only one of the nine equally likely pairs is forbidden. This is the case with success [probability](../../../../../../probability.md) $1/3$ of the [avoidance recurrence for two consecutive successes](../../../../../../avoidance-recurrence-for-two-consecutive-successes.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
