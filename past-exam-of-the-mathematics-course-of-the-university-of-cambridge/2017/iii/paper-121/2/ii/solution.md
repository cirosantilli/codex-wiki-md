<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix the base convention $L_0(X)=X$. For a [transitive set](../../../../../../transitive-set.md) $X$, the [relative constructible hierarchy](../../../../../../relative-constructible-hierarchy.md) is

$$
\boxed{L_0(X)=X,\qquad L_{\alpha+1}(X)=\operatorname{Def}(L_\alpha(X)),\qquad L_\lambda(X)=\bigcup_{\alpha<\lambda}L_\alpha(X),\qquad L(X)=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha(X).}
$$

Here the [definable power set](../../../../../../definable-power-set-split.md) is

$$
\operatorname{Def}(A)=\{\{u\in A:(A,\in)\models\varphi(u,\vec a)\}:\varphi\text{ a first-order formula},\ \vec a\in A^{<\omega}\}.
$$

The [satisfaction for a set structure](../../../../../../satisfaction-for-a-set-structure.md) in this definition is a definable set-theoretic relation, obtained by finite syntax coding and recursion on a [first-order formula](../../../../../../first-order-formula.md). The [transfinite recursion](../../../../../../transfinite-recursion.md) therefore defines a class in [ZF](../../../../../../zermelo-fraenkel-set-theory.md).

Each level is a [transitive set](../../../../../../transitive-set.md). For transitive $A$, every $a\in A$ is a [subset](../../../../../../subset.md) of $A$ definable using the parameter $a$, so $A\subseteq\operatorname{Def}(A)$; also $A\in\operatorname{Def}(A)$ using the always-true [first-order formula](../../../../../../first-order-formula.md). Thus the levels increase and $X\in L_1(X)$. Starting instead with $X\cup\{X\}$ is another common indexing convention, but it is not the convention used here. The relative universe need not satisfy [axiom of choice](../../../../../../axiom-of-choice.md): arbitrary $X$ need not have an internally available [well-order](../../../../../../well-order.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
