<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Add a stratum indicator that is “First” for the first episode and “Later” for every subsequent episode, including the final censored episode:

| Patient | Next-event episode | Gap start | Gap stop | Event | $z$ | Stratum |
| --- | --- | --- | --- | --- | --- | --- |
| 001 | 1 | 0 | 24.8 | 1 | 0 | First |
| 001 | 2 | 3 | 8.3 | 1 | 0 | Later |
| 001 | 3 | 3 | 7.1 | 1 | 0 | Later |
| 001 | 4 | 3 | 11.7 | 1 | 0 | Later |
| 001 | 5 | 3 | 8.1 | 0 | 0 | Later |

A [Stratified Cox model](../../../../../../stratified-cox-model.md) then uses distinct [baseline hazards](../../../../../../baseline-hazard.md) $h_{0,\mathrm{first}}$ and $h_{0,\mathrm{later}}$, with a common treatment coefficient $\beta$ unless an interaction is explicitly desired. Form separate [risk sets](../../../../../../risk-set.md) within the two strata and multiply their partial [likelihoods](../../../../../../likelihood-function.md). There is no need to force every later event number to have its own baseline when the stated aim is only first versus subsequent headaches. This is a [first-event versus recurrent-event baseline stratification](../../../../../../first-event-versus-recurrent-event-baseline-stratification.md).

## ↑ Ancestors (11)

1. [E](../e.md)
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
