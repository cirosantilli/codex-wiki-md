<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Iterating the [CUSUM](../../../../../../cusum.md) recursion shows that

$$
X_t=\max\left(0,\max_{1\leq k\leq t}\sum_{s=k}^tW_s\right).
$$

Thus it searches all possible starting times for a recent stretch of evidence favoring an increase. If adding an increment makes the current sum negative, that accumulated evidence favors the null; retaining it would force a later real deterioration first to repay a deficit accumulated during healthy years. Starting a new candidate segment gives zero instead. **Resetting at zero makes detection responsive to a change with unknown onset.** Negative values would be permissible for a fixed-start signed [log-likelihood ratio](../../../../../../log-likelihood-ratio.md), but that is a different statistic from this one-sided tabular [CUSUM](../../../../../../cusum.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
