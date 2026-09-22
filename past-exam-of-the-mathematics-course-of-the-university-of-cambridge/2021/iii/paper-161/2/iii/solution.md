<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose $A$ uniformly from $\mathcal A$, and let $X_i=\mathbf1_{\{i\in A\}}$. The [characteristic vector of a set](../../../../../../characteristic-vector-of-a-set.md) determines $A$, so

$$
H(X_1,ldots,X_n)=\log|\mathcal A|.
$$

For $F\in\mathcal F$, the projected vector $X_F$ determines the intersection $A\cap F$ and therefore takes values in the [trace of a set family](../../../../../../trace-of-a-set-family.md) $T_F(\mathcal A)$. The maximum-entropy bound on a finite set gives

$$
H(X_F)\leq\log|T_F(\mathcal A)|.
$$

Every coordinate belongs to at least $t$ members of $\mathcal F$, so [Shearer's inequality](../../../../../../shearer-s-inequality.md) gives

$$
t\log|\mathcal A|
\leq\sum_{F\in\mathcal F}\log|T_F(\mathcal A)|.
$$

Exponentiation proves the [Shearer trace inequality](../../../../../../shearer-trace-inequality.md)

$$
\boxed{|\mathcal A|\leq
\left(\prod_{F\in\mathcal F}|T_F(\mathcal A)|\right)^{1/t}}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
