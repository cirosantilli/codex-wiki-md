<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Call the parent [genotype](../../../../../../genotype.md) $g$ and child [genotype](../../../../../../genotype.md) $h$, each in $\{0,1\}$. Define

$$
a_g=P(X_p\mid G_p=g),\quad p_g=P(G_p=g),\quad
b_h=P(X_c\mid G_c=h),\quad t_{h\mid g}=P(G_c=h\mid G_p=g).
$$

There is one [pedigree founder](../../../../../../founder-in-a-pedigree.md) and one nonfounder, so

$$
\boxed{L=\sum_{g=0}^1\sum_{h=0}^1 a_gp_gb_ht_{h\mid g}.}
$$

Explicitly this is $a_0p_0b_0t_{0\mid0}+a_0p_0b_1t_{1\mid0}+a_1p_1b_0t_{0\mid1}+a_1p_1b_1t_{1\mid1}$. The genotype-transmission model can be arbitrary for the single-parent species; no two-parent Mendelian assumption is being introduced.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
