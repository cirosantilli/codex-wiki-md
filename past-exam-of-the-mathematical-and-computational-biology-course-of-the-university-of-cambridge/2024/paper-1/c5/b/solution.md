<h1 id="c5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Count the number of descendant leaves on each branch during each [phylogenetic epoch](../../../../../phylogenetic-epoch.md). From the tips backward, both topologies have branch-size lists $(1,1,1,1)$ during $T_4$, then $(2,1,1)$ during $T_3$. During $T_2$, type A has $(3,1)$ and type B has $(2,2)$.

Let $L_j$ be the total length of branches carrying $j$ descendant leaves. Adding the relevant [phylogenetic epoch](../../../../../phylogenetic-epoch.md) durations gives

$$
\boxed{\begin{array}{c|ccc}
&\mathbb E[L_1]&\mathbb E[L_2]&\mathbb E[L_3]\\\hline
A&4E_4+2E_3+E_2&E_3&E_2\\
B&4E_4+2E_3&E_3+2E_2&0
\end{array}}.
$$

For example, type A has one external branch and one three-descendant branch throughout $T_2$, while type B has two two-descendant branches. In either case the total expected branch length is $4E_4+3E_3+2E_2$, a useful accounting check. The stem above the common root is excluded because [mutations](../../../../../mutation.md) there would be shared by all four samples.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [C5](../../c5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
