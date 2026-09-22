<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At day 165 there are two A and two B individuals at risk. The event is in A, with expected A count $2/4=1/2$, so its score contribution is $1-1/2=1/2$ and its [variance](../../../../../../variance-split.md) contribution is $1/4$. The remaining A individual is censored at 173 and leaves the [risk set](../../../../../../risk-set.md) before either later event. The risk-set calculations are

| Event day | $n_A$ | $n_B$ | $d_A$ | $e_A$ | $d_A-e_A$ | Variance |
| --- | --- | --- | --- | --- | --- | --- |
| 165 | 2 | 2 | 1 | $1/2$ | $1/2$ | $1/4$ |
| 180 | 0 | 2 | 0 | 0 | 0 | 0 |
| 191 | 0 | 1 | 0 | 0 | 0 | 0 |

Thus

$$
\boxed{U_{A,>160}=\frac12,\qquad V_{>160}=\frac14.}
$$

The positive score indicates higher A event hazard in this late contribution. Although B has more observed events, its two events occur with no A individual at risk, so those times do not compare the groups. This is why raw event totals alone are insufficient for the [log-rank test](../../../../../../log-rank-test.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
