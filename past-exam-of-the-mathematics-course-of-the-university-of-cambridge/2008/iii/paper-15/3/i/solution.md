<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Balister-Bollobas inequality](../../../../../../balister-bollobas-entropy-inequality.md) says that if $r_i$ is the coordinate multiplicity in a multiset $\mathcal A$, and $L_j=\{i:r_i\geq j\}$, then $\sum_jH(X_{L_j})\leq\sum_{A\in\mathcal A}H(X_A)$. More generally, each union-intersection compression decreases the entropy sum, by [entropy submodularity](../../../../../../entropy-submodularity.md).

For an exact $k$-cover define $A^-=[\min A-1]$ and $A^+=[\max A-1]\setminus A$. Compressing the family of $A\cup A^-$ gives the nested family of all $A^-$ together with $k$ full sets. Rearranging the resulting bound gives the upper [Madiman-Tetali inequality](../../../../../../madiman-tetali-entropy-inequality.md). Conversely, compressing the family of all $A^+$ together with $k$ full sets gives the nested family of $A\cup A^+$, yielding the lower bound. In conditional-entropy notation these are

$$
\boxed{\sum_{A\in\mathcal A}H(X_A\mid X_{A^+})\leq kH(X)\leq\sum_{A\in\mathcal A}H(X_A\mid X_{A^-}).}
$$

The coordinate multiplicities agree in each compression, because $\mathcal A$ is an exact $k$-cover. An equivalent proof expands the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) contributions $h_i=H(X_i\mid X_{[i-1]})$ and uses [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md). It also gives the upper inequality for arbitrary fractional covers and the lower inequality for fractional packings.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
