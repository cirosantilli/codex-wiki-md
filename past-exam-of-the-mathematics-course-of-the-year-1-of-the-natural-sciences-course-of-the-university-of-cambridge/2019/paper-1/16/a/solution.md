<h1 id="16/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the intended model of uniform draws and a replacement decision independent of the first ball's colour, with [probability](../../../../../probability.md) $r$. The marginal specification $P(R)=r$ alone would not determine the experiment if replacement depended on that colour. This independence assumption is used throughout the question.

Write $\overline B_j$ for a non-blue draw and $\overline R$ for no replacement. The [sample space](../../../../../sample-space.md) consists of the eight ordered outcomes obtained by choosing one of $B_1,\overline B_1$, then one of $R,\overline R$, then one of $B_2,\overline B_2$. The [chain rule for probabilities](../../../../../chain-rule-for-probabilities.md) gives their [probabilities](../../../../../probability.md):

$$
\boxed{\begin{array}{c|c}
\text{outcome}&\text{probability}\\\hline
B_1\cap R\cap B_2&4r/25\\
B_1\cap R\cap\overline B_2&6r/25\\
\overline B_1\cap R\cap B_2&6r/25\\
\overline B_1\cap R\cap\overline B_2&9r/25\\
B_1\cap\overline R\cap B_2&(1-r)/10\\
B_1\cap\overline R\cap\overline B_2&3(1-r)/10\\
\overline B_1\cap\overline R\cap B_2&3(1-r)/10\\
\overline B_1\cap\overline R\cap\overline B_2&3(1-r)/10
\end{array}}
$$

For example, the first entry is $(2/5)r(2/5)$. The fifth is $(2/5)(1-r)(1/4)$ because one blue ball has been removed. With no replacement after a non-blue first draw, the two remaining colours each have two balls, explaining the last two entries. The first four entries sum to $r$ and the last four to $1-r$, so the full [sample space](../../../../../sample-space.md) has total [probability](../../../../../probability.md) one. At $r=0$ or $1$, the corresponding impossible outcomes simply have zero [probability](../../../../../probability.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [16](../../16.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
