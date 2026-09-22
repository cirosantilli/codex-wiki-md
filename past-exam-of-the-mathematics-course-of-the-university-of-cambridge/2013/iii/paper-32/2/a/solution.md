<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Label batches before consulting the random-number table, so their labels are independent of the test results. A uniformly random permutation of $1,\ldots,16$, restricted to a smaller label set, induces a uniformly random ordering of that set. This provides a simple rejection-and-restriction scheme:

- For A, label each day's six batches $1,\ldots,6$. Use a fresh permutation, discard labels $7,\ldots,16$, and test the first remaining batch. Repeat independently on each working day. Each daily batch has inclusion [probability](../../../../../../probability.md) $1/6$, and five batches are tested per week.
- For B, label the fifteen weekly morning batches $1,\ldots,15$. Discard label 16 from a fresh permutation and choose the first three remaining labels. Use an independent permutation for the afternoon stratum. Every three-element subset within a stratum is equally likely, and each batch has inclusion [probability](../../../../../../probability.md) $3/15=1/5$. Six batches are tested per week.
- For C, label the weekdays $1,\ldots,5$. Keep the first label in this range from a fresh permutation and test all six batches on that day. Repeat independently each week. Every day, and hence every batch, has inclusion [probability](../../../../../../probability.md) $1/5$; six batches are tested per week.

With independent random digits instead, [rejection sampling](../../../../../../rejection-sampling.md) gives the same uniform choices: for A keep only digits $1,\ldots,6$; for C keep only $1,\ldots,5$. For B, use uniform two-digit numbers, retain labels $01,\ldots,15$, and reject repeats within a three-batch sample. Taking residues modulo six or fifteen from a table whose range is not divisible by that number would give unequal [probabilities](../../../../../../probability.md). These are respectively day-stratified [simple random sampling](../../../../../../simple-random-sampling.md), morning/afternoon [stratified sampling](../../../../../../stratified-sampling.md), and a one-day design using [cluster sampling](../../../../../../cluster-sampling.md). The printed word “rest” for A is interpreted as “test”, consistently with the surveillance task. If it instead meant leaving one batch untested, choose that omitted batch uniformly and test the other five; this alternative would test 25 batches per week, with inclusion [probability](../../../../../../probability.md) $5/6$, and has a different testing budget.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
