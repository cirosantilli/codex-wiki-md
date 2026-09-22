<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $S_i=[n]\setminus\{i\}$, the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) gives

$$
H(X_{S_i})=\sum_{j\in S_i}H(X_j\mid X_{S_i\cap[j-1]}).
$$

Each summand is at least $H(X_j\mid X_1^{j-1})$ because [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md). Summing over $i$, each $j$ occurs $n-1$ times:

$$
\sum_{i=1}^nH(X_{S_i})
\geq(n-1)\sum_{j=1}^nH(X_j\mid X_1^{j-1})
=(n-1)H(X_1^n).
$$

This is the required special case of [Shearer's inequality](../../../../../../shearer-s-inequality.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
