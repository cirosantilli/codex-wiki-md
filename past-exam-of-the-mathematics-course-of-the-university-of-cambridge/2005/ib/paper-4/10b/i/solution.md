<h1 id="10b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Apply the [Gram-Schmidt process](../../../../../../gram-schmidt-process.md) explicitly. Start with $f_1=e_1/\|e_1\|$, and for $i\geq2$ set

$$
v_i=e_i-\sum_{j=1}^{i-1}\langle e_i,f_j\rangle f_j,\qquad f_i=v_i/\|v_i\|.
$$

Assume inductively that the previous $f_j$ form an [orthonormal basis](../../../../../../orthonormal-basis.md) for the span of $e_1,\ldots,e_{i-1}$. [Inner products](../../../../../../inner-product.md) give $\langle v_i,f_j\rangle=0$ for every $j<i$. Moreover $v_i\ne0$: otherwise $e_i$ would lie in the span of its predecessors, contradicting that the $e_j$ form a [basis](../../../../../../basis.md). Thus $f_i$ is well defined and has unit [norm](../../../../../../norm.md). The definition expresses $f_i$ in the span of $e_1,\ldots,e_i$, and also expresses $e_i$ in the span of $f_1,\ldots,f_i$. The two spans therefore agree at each stage. Induction proves **the required orthonormal, span-preserving basis**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10B](../../10b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
