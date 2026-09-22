<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For second and subsequent episodes, subtract the preceding headache time from both calendar endpoints. The new clock is the age since the start of that headache, not the age since recovery ended. Keeping the recovery restriction from part (c) therefore gives

| Patient | Next-event episode | Gap start | Gap stop | Event | $z$ |
| --- | --- | --- | --- | --- | --- |
| 001 | 1 | 0 | 24.8 | 1 | 0 |
| 001 | 2 | 3 | 8.3 | 1 | 0 |
| 001 | 3 | 3 | 7.1 | 1 | 0 |
| 001 | 4 | 3 | 11.7 | 1 | 0 |
| 001 | 5 | 3 | 8.1 | 0 | 0 |

For example, the second stop is $33.1-24.8=8.3$, while its entry is $27.8-24.8=3$. Thus subsequent rows begin at gap age three, not zero. The first row retains time since treatment started. Keep the patient and episode labels, and preferably the original calendar endpoints as auxiliary fields: gap ages in different episodes are not chronological treatment times. The value 7.1 for episode three being smaller than 8.3 for episode two does not reverse their occurrence order. This [gap-time recurrent-event model](../../../../../../gap-time-recurrent-event-model.md) forms [risk sets](../../../../../../risk-set.md) on the episode-age scale while preserving each episode's historical eligibility.

## ↑ Ancestors (11)

1. [D](../d.md)
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
