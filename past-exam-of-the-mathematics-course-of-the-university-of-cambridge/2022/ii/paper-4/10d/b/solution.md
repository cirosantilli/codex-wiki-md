<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $n$ [controlled-NOT gates](../../../../../../controlled-not-gate.md) in parallel. For each $j=1,\ldots,n$, the $j$th input qubit is the control and the $j$th output-register qubit is the target. Their combined action is

$$
|x_1\cdots x_n\rangle|y_1\cdots y_n\rangle
\longmapsto
|x_1\cdots x_n\rangle
|y_1\mathbin\oplus x_1,\ldots,y_n\mathbin\oplus x_n\rangle,
$$

which is exactly

$$
\boxed{|x\rangle|y\rangle\mapsto|x\rangle|y\mathbin\oplus x\rangle=U_{\mathcal I}|x\rangle|y\rangle}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
