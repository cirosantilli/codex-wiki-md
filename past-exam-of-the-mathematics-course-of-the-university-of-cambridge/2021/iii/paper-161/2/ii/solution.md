<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Shearer's inequality](../../../../../../shearer-s-inequality.md) states that if $X=(X_1,\ldots,X_n)$ is a discrete [random vector](../../../../../../random-vector.md) and $\mathcal F$ is a collection of subsets of $[n]$ in which every index occurs at least $t$ times, then

$$
\boxed{tH(X)\leq\sum_{F\in\mathcal F}H(X_F)}.
$$

Order the coordinates naturally. For every $F\in\mathcal F$, the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) gives

$$
H(X_F)=\sum_{i\in F}H\left(X_i\mid X_j:j\in F,\ j<i\right).
$$

Removing conditioning variables cannot decrease entropy, so every summand is at least

$$
H(X_i\mid X_1,\ldots,X_{i-1}).
$$

After summing over $F$, each index $i$ contributes at least $t$ times. A final application of the chain rule yields

$$
\sum_{F\in\mathcal F}H(X_F)
\geq t\sum_{i=1}^nH(X_i\mid X_1,\ldots,X_{i-1})
=tH(X),
$$

which proves the lemma.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 161](../../../paper-161-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
