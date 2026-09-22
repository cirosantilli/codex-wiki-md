<h1 id="12h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Rice theorem](../../../../../../rice-s-theorem.md) says that every nontrivial [extensional property of programs](../../../../../../extensional-property-of-programs.md) computing partial functions is undecidable. Equivalently, a nontrivial [index set](../../../../../../index-set.md) cannot be a [computable set](../../../../../../computable-set.md).

Let $A$ be such an index set. Replacing $A$ by its complement if necessary, assume that the nowhere-defined function has no index in $A$. Since the property is nontrivial, choose an index $a\in A$. If membership in $A$ were decidable, we could decide the diagonal [halting problem](../../../../../../halting-problem.md) as follows. For each $x$, define

$$
\psi_x(y)\simeq
\begin{cases}
f_{a,1}(y),&\text{after the computation }f_{x,1}(x)\text{ halts},\\
\text{undefined},&\text{if that computation never halts}.
\end{cases}
$$

By the [S-m-n theorem](../../../../../../smn-theorem.md), a total computable function $q$ produces an index $q(x)$ for $\psi_x$. If $f_{x,1}(x)$ diverges, then $\psi_x$ is nowhere defined and $q(x)\notin A$. If it halts, then $\psi_x\simeq f_{a,1}$ and extensionality gives $q(x)\in A$. A decider for $A$ would therefore decide whether $f_{x,1}(x)$ halts, a contradiction. Hence $A$ is undecidable.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12H](../../12h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
