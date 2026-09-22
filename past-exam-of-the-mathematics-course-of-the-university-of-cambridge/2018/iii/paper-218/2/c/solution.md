<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a candidate grid of $C>0$. For each candidate and each $i$, fit the [soft-margin support vector machine](../../../../../../soft-margin-support-vector-machine.md) to all observations except $i$, keeping exactly the same $C$ in the unnormalized sum objective. Let $f_{-i,C}$ be its fitted score. Use a fixed rule for assigning a label when the score is zero. The binary misclassification estimate from [Leave-one-out cross-validation](../../../../../../leave-one-out-cross-validation.md) is

$$
\boxed{\operatorname{err}_{CV}(C)=\frac1n\sum_{i=1}^n\mathbf1_{\{\operatorname{sign}(f_{-i,C}(x_i))\ne y_i\}}.}
$$

Choose a minimizing candidate, break tuning ties by a predetermined rule, and refit on all $n$ observations. Any estimated preprocessing must also be fitted inside each training fold to avoid [data leakage](../../../../../../data-leakage.md). If a normalized average-loss parameterization is used instead, translate its parameter so that the same $C$ is retained when the sample size decreases.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
