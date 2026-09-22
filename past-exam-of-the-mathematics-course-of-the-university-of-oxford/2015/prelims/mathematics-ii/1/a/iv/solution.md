<h1 id="1/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If $a_n\to L$, every [subsequence](../../../../../../../subsequence.md) also has [limit of a sequence](../../../../../../../limit-of-a-sequence.md) $L$: its increasing indices eventually exceed any prescribed threshold. This applies in particular to every [monotone subsequence](../../../../../../../monotone-subsequence.md).

Conversely, suppose $(a_n)$ is a [bounded sequence](../../../../../../../bounded-sequence.md) and all its [monotone subsequences](../../../../../../../monotone-subsequence.md) converge to the same $L$. At least one exists by the [monotone subsequence theorem](../../../../../../../monotone-subsequence-theorem.md). If $a_n$ did not tend to $L$, there would be $\varepsilon_0>0$ and a [subsequence](../../../../../../../subsequence.md) $(a_{n_j})$ such that

$$
|a_{n_j}-L|\geq\varepsilon_0\qquad(j\geq1).
$$

Apply the [monotone subsequence theorem](../../../../../../../monotone-subsequence-theorem.md) to $(a_{n_j})$. The resulting further [subsequence](../../../../../../../subsequence.md) is also a [monotone subsequence](../../../../../../../monotone-subsequence.md) of $(a_n)$, so it tends to $L$, contradicting the displayed bound. Therefore

$$
\boxed{a_n\to L\ \Longleftrightarrow\ \text{every monotone subsequence tends to }L.}
$$

The [bounded monotone sequence theorem](../../../../../../../bounded-monotone-sequence-theorem.md) ensures that these [subsequences](../../../../../../../subsequence.md) have finite [limits of sequences](../../../../../../../limit-of-a-sequence.md); the hypothesis requires those values to agree.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
