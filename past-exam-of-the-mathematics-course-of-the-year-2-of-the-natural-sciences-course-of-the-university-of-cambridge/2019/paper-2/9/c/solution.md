<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) found in part (b) is the translation subgroup

$$
\boxed{N=\ker f=\left\{T_c=\begin{pmatrix}1&c\\0&1\end{pmatrix}:c\in\mathbb C\right\}}.
$$

It is a [subgroup](../../../../../subgroup.md) because $T_cT_d=T_{c+d}$, $T_0=I$ and $T_c^{-1}=T_{-c}$. It is nontrivial since $T_1\ne I$, and proper since, for example, $M(2,0)\notin N$.

Every kernel is a [normal subgroup](../../../../../normal-subgroup.md): if $n\in\ker f$, then $f(gng^{-1})=f(g)e f(g)^{-1}=e$. Applying the same argument with $g^{-1}$ gives equality of the conjugate subgroup and the kernel. Here one can also check invariance under [conjugation](../../../../../conjugation.md) directly:

$$
M(a,b)T_cM(a,b)^{-1}=T_{ac}.
$$

Multiplication by nonzero $a$ permutes all $c\in\mathbb C$, so $M(a,b)NM(a,b)^{-1}=N$. Thus $N$ is a nontrivial proper [normal subgroup](../../../../../normal-subgroup.md), [isomorphic](../../../../../isomorphism.md) to the additive [group](../../../../../group-split.md) $(\mathbb C,+)$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
