<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $a=\beta^*=\beta N+\gamma$. If the first event is recovery, the epidemic has ended and a second event is impossible. If the first event is infection at time $s$, its density is $\beta N e^{-as}$, and the new state is $(N-1,2,0)$. The total next-event rate is

$$
b=2\beta(N-1)+2\gamma=2(a-\beta).
$$

Thus, by the [Markov property](../../../../../../markov-property.md), **the [two-event probability in a stochastic SIR model](../../../../../../two-event-probability-in-a-stochastic-sir-model.md) by time one** is

$$
\int_0^1\beta N e^{-as}\left(1-e^{-b(1-s)}\right)\,ds.
$$

Evaluate the first term as $\beta N(1-e^{-a})/a$. For the second, $b-a=a-2\beta$, so

$$
\int_0^1\beta N e^{-as-b(1-s)}\,ds=\frac{\beta N e^{-a}}{a-2\beta}\left(1-e^{-(a-2\beta)}\right).
$$

Therefore

$$
\boxed{\mathbb P(\text{at least two events in }[0,1))=\frac{\beta N}{\beta^*}(1-e^{-\beta^*})-\frac{\beta N e^{-\beta^*}}{\beta^*-2\beta}(1-e^{-(\beta^*-2\beta)}).}
$$

For $N\ge2$ and $\gamma>0$, the denominator $\beta^*-2\beta=\beta(N-2)+\gamma$ is positive. Event times are continuous, so inclusion or exclusion of the endpoint one makes no difference.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
