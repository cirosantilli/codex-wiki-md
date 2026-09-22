<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes.** Start with the model $M_0$ constructed in part a. If $M_0$ has no internally [strongly inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md) above $\kappa$, put $M=M_0$. Otherwise let $\delta$ be the least ordinal above $\kappa$ that $M_0$ regards as strongly inaccessible, and put

$$
M=(V_\delta)^{M_0}.
$$

In the second case $M\models\mathrm{ZFC}$ because $M_0$ regards $\delta$ as inaccessible. The measure witnessing that $\kappa$ is [measurable](../../../../../../measurable-cardinal.md) has rank below $\kappa+3<\delta$, so it still belongs to $M$. In both cases $M$ is a [transitive set](../../../../../../transitive-set.md) of cardinality $\kappa$, contains $V_\kappa$, and has no internally inaccessible ordinal strictly between $\kappa$ and its height.

We verify [absoluteness](../../../../../../set-theoretic-absoluteness.md) for every ordinal $\alpha\in M$. If $\alpha<\kappa$, then $M$ and $V_\lambda$ both contain $V_{\alpha+1}$ and therefore compute all subsets and functions relevant to strong inaccessibility in the same way. At $\alpha=\kappa$, both models see a [measurable cardinal](../../../../../../measurable-cardinal.md) and hence an inaccessible cardinal. Finally, if $\kappa<\alpha\in M$, then $M$ says that $\alpha$ is not inaccessible by construction. The larger model $V_\lambda$ cannot say that it is inaccessible, because strong inaccessibility is downward absolute to a transitive model of ZFC: any failure visible in the smaller model remains a failure in the larger one, while ambient inaccessibility would force internal inaccessibility. Hence “$\alpha$ is inaccessible” is absolute between $M$ and $V_\lambda$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 116](../../../paper-116-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
