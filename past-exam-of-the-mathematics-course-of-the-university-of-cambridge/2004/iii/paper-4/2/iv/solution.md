<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Choose a finite set $S$ of [topological generators](../../../../../../topological-generator.md) of $G$ and let $\Gamma=\langle S\rangle$ denote the abstract subgroup it generates. Then $\Gamma$ is dense in $G$. For an [open subgroup](../../../../../../open-subgroup.md) $H$, the abstract subgroup $K=\Gamma\cap H$ is dense in $H$, since every nonempty open subset of $H$ is open in $G$. Every coset of $H$ meets $\Gamma$, so $[\Gamma:K]=[G:H]=m<\infty$.

Here is the needed [Schreier lemma](../../../../../../reidemeister-schreier-theorem.md) argument explicitly. Choose representatives $t$ in $\Gamma$ for the right [cosets](../../../../../../coset.md) $K\backslash\Gamma$, including $1$ for $K$, and write $\overline\gamma$ for the representative of $K\gamma$. The finite set

$$
\{t s\,\overline{ts}^{-1}:t\text{ a representative},\ s\in S\cup S^{-1}\}
$$

is contained in $K$. For $k=s_1\cdots s_r\in K$, set $t_j=\overline{s_1\cdots s_j}$, with $t_0=t_r=1$. Then

$$
k=\prod_{j=1}^r(t_{j-1}s_jt_j^{-1}),
$$

and every factor belongs to the displayed finite set. Thus $K$ is finitely generated as an abstract [group](../../../../../../group-split.md). Its finite generators topologically generate its closure $H$. **Every open subgroup of a finitely generated profinite group is finitely generated.**

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
