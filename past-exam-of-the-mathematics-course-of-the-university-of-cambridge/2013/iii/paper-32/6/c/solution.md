<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set the availability indicator $Y_i(t)$ to zero during the three-day recovery interval after each headache. Keep each episode's endpoint, but delay its entry to the previous headache time plus three. The calendar-time rows become

| Patient | Next-event episode | Start | Stop | Event | $z$ |
| --- | --- | --- | --- | --- | --- |
| 001 | 1 | 0 | 24.8 | 1 | 0 |
| 001 | 2 | 27.8 | 33.1 | 1 | 0 |
| 001 | 3 | 36.1 | 40.2 | 1 | 0 |
| 001 | 4 | 43.2 | 51.9 | 1 | 0 |
| 001 | 5 | 54.9 | 60.0 | 0 | 0 |

The first interval still begins at zero because the patient was already headache-free for at least seven days before treatment. The recovery gaps supply no at-risk exposure and no partial-[likelihood](../../../../../../likelihood-function.md) risk-set membership; they should not be retained as ordinary event-free at-risk time. If recovery extends past administrative closure, no subsequent eligible interval is created. This is a [refractory period in recurrent-event analysis](../../../../../../refractory-period-in-recurrent-event-analysis.md), represented by availability rather than by changing the event times.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
