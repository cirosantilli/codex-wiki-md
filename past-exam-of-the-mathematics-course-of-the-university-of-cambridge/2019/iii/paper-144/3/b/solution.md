<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $B=N\setminus\operatorname{acl}(A)$. We seek a model containing $A$ and omitting every element of $B$. Every finite set of these omission requirements is satisfiable: if a finite $C\subseteq B$ met every model containing $A$, the supplied result would imply $C\cap\operatorname{acl}(A)\ne\varnothing$, a contradiction.

Apply the [compactness theorem](../../../../../../compactness-theorem.md) to the elementary-diagram formulation of these requirements, using the [Tarski-Vaught test](../../../../../../tarski-vaught-test.md) to axiomatize the selected elementary submodel. It gives a model $M$ containing $A$ and omitting all of $B$. Part (a) gives $\operatorname{acl}(A)\subseteq M\cap N$, while omission of $B=N\setminus\operatorname{acl}(A)$ gives the reverse inclusion. Therefore

$$
\boxed{M\cap N=\operatorname{acl}(A).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 144](../../../paper-144-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
