<h1 id="2/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We prove simultaneously that each $L_\alpha$ is a [transitive set](../../../../../../../transitive-set.md) and that $L_\alpha\subseteq L_{\alpha+1}$. The key observation is that if $A$ is transitive and $x\in A$, then $x\subseteq A$ and

$$
x=\{y\in A:(A,\in)\models y\in x\}.
$$

This is an internal definition with parameter $x$, so $x\in\operatorname{Def}(A,1)$. Hence $A\subseteq\operatorname{Def}(A,1)$. Every $z\in\operatorname{Def}(A,1)$ is a subset of $A$; if $y\in z$, then $y\in A\subseteq\operatorname{Def}(A,1)$. Thus the definable power set is transitive too.

Start with the empty set. At successor stages the observation proves transitivity and inclusion. At a limit stage the union of the earlier transitive sets is transitive, and the same observation then proves its inclusion in its own definable power set. This completes the [transfinite induction](../../../../../../../transfinite-induction.md) and gives

$$
\boxed{\forall\alpha\quad L_\alpha\text{ is transitive}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
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
