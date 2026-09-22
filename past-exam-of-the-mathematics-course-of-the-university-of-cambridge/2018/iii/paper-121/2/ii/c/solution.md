<h1 id="2/ii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Induct on $\alpha$ using the transitivity and inclusion already established. The zero stage is immediate. Suppose $L_\alpha\cap\operatorname{Ord}=\alpha$. Being an [ordinal](../../../../../../../ordinal.md) is expressible by a [bounded formula in set theory](../../../../../../../bounded-formula-in-set-theory.md), for example transitivity, transitivity of all members, and membership comparability. It is therefore absolute for the transitive set $L_\alpha$. The subset of its elements that are ordinals is internally definable, so

$$
\alpha=\{x\in L_\alpha:x\text{ is an ordinal}\}\in\operatorname{Def}(L_\alpha,1)=L_{\alpha+1}.
$$

By inclusion, all smaller ordinals are present as well. Conversely, if an ordinal $\gamma$ belongs to $L_{\alpha+1}$, then $\gamma\subseteq L_\alpha$, since every member of a [definable power set](../../../../../../../definable-power-set-split.md) is a subset of the preceding domain. All members of $\gamma$ are ordinals, so $\gamma\subseteq L_\alpha\cap\operatorname{Ord}=\alpha$ and $\gamma\leq\alpha$. Hence the ordinal part of the successor level is exactly $\alpha+1$.

At a nonzero limit ordinal $\lambda$,

$$
L_\lambda\cap\operatorname{Ord}=\bigcup_{\alpha<\lambda}(L_\alpha\cap\operatorname{Ord})=\bigcup_{\alpha<\lambda}\alpha=\lambda.
$$

Thus

$$
\boxed{L_\alpha\cap\operatorname{Ord}=\alpha\quad\text{for every ordinal }\alpha.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Ii](../../ii.md)
3. [2](../../../2.md)
4. [Paper 121](../../../../paper-121-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
