<h1 id="3/iii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [early stopping of Landweber iteration](../../../../../../../early-stopping-of-landweber-iteration.md). For each finite $n$, the [Landweber spectral filter](../../../../../../../landweber-spectral-filter.md) gives a bounded reconstruction operator; as $n\to\infty$, it approaches the generalized inverse on exact admissible data. Taking $\alpha=1/n$, a sufficient rule for a [convergent regularization of an inverse problem](../../../../../../../convergent-regularization-of-an-inverse-problem.md) is

$$
\boxed{n(\delta)\to\infty,\qquad \sqrt{n(\delta)}\,\delta\to0,}
$$

or equivalently $\alpha(\delta)\to0$ and $\delta/\sqrt{\alpha(\delta)}\to0$. For example, $n(\delta)=\lfloor\delta^{-1}\rfloor$ satisfies both in the normalized problem. The first condition removes exact-data bias; the second prevents arbitrarily small measurement errors from being amplified by excessive iteration.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Iii](../../iii.md)
3. [3](../../../3.md)
4. [Paper 335](../../../../paper-335-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
