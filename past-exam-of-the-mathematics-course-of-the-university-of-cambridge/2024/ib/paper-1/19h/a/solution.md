<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Starting from $i$, the probability of reaching $j$ before returning to $i$ is $\alpha$. Conditional on reaching $j$, each visit to $j$ is followed by a hit on $i$ before the next return to $j$ with probability $\alpha$, by symmetry and the [Strong Markov property](../../../../../../strong-markov-property.md). For $\alpha>0$, the number of visits after entry is therefore geometric on $\{1,2,\ldots\}$ with mean $1/\alpha$. Hence the [two-state excursion visit law](../../../../../../two-state-excursion-visit-law.md) gives

$$
\boxed{\mathbb E_iN=\alpha\frac1\alpha=1}
\qquad(\alpha>0).
$$

In the degenerate case $\alpha=0$, the chain never reaches $j$ before its return to $i$, so $N=0$ almost surely and $\mathbb E_iN=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
