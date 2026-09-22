<h1 id="20c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On the negative branch set $Y=-X$. Its outward step probability is $3/4$ and inward probability is $1/4$. The same finite [gambler's ruin](../../../../../../gambler-s-ruin.md) recurrence as in part (a), with root $(1/4)/(3/4)=1/3$, gives $\Pr_{-1}(T_0<\infty)=1/3$. Hence, following one departure from zero, the probability of returning is

$$
r=\frac12\cdot\frac12+\frac12\cdot\frac13=\frac5{12}<1.
$$

At each return the [Strong Markov property](../../../../../../strong-markov-property.md) restarts the same excursion experiment. The probability of at least $m$ returns is $r^m$, tending to zero. Thus almost surely there is a last visit to zero.

After that visit the walk remains strictly positive or strictly negative, because nearest-neighbour steps cannot change sign without crossing zero. On the positive branch it can be coupled, up to any return, to independent steps of mean $2/3-1/3=1/3$. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives a walk tending to $+\infty$ almost surely. This conclusion remains true on the event that the excursion never returns: conditioning on a positive-probability event cannot make a probability-zero failure of the law occur. On the negative branch the mean step is $1/4-3/4=-1/2$, giving $-\infty$ in the same way. Apply this at each possible departure time, a countable family, or use the [Strong Markov property](../../../../../../strong-markov-property.md) at the successive returns. Therefore

$$
\boxed{\Pr_0(X_n\to+\infty\ \hbox{or}\ X_n\to-\infty)=1.}
$$

Finite visits to zero alone would not prove divergence on an arbitrary chain; the outward-drift argument is the additional step needed here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20C](../../20c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
