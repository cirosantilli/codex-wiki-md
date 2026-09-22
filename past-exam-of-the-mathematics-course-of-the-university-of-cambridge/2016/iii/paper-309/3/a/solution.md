<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $V=T_p\mathcal M$ and $V^*$ for its [dual space](../../../../../../dual-space.md). A type-$(1,1)$ [tensor](../../../../../../tensor.md) is equivalently a [linear map](../../../../../../linear-map.md) $A:V\to V$: the corresponding scalar-valued [multilinear map](../../../../../../multilinear-map.md) is $(X,\eta)\mapsto\eta(A(X))$. Thus the composition defines

$$
C(X,\eta)=\eta\bigl(B(A(X))\bigr).
$$

It is linear in $X$ because $A$ and $B$ are [linear maps](../../../../../../linear-map.md), and linear in the [covector](../../../../../../covector.md) $\eta$ by evaluation. This proves directly that **the composition is a tensor of type $(1,1)$**.

Choose a basis $e_\alpha$ of the [tangent space](../../../../../../tangent-space.md) and its dual basis $e^\beta$. With the paper's component order $A(e_\alpha)=A_\alpha{}^\gamma e_\gamma$,

$$
B(A(e_\alpha))=A_\alpha{}^\gamma B_\gamma{}^\beta e_\beta,
\qquad
\boxed{C_\alpha{}^\beta=A_\alpha{}^\gamma B_\gamma{}^\beta.}
$$

Equivalently, in the usual output-first matrix notation, $C^\beta{}_\alpha=B^\beta{}_\gamma A^\gamma{}_\alpha$: **the matrix product is $BA$, not $AB$**. This [composition of mixed tensors](../../../../../../composition-of-mixed-tensors.md) contracts one output index with one input index. Under the [tensor component transformation law](../../../../../../tensor-component-transformation-law.md), the two Jacobian factors at that contracted index cancel, leaving exactly one factor for each free index.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
