<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Proceed by [structural induction](../../../../../../structural-induction.md) on a Boolean formula $F$. A leaf computes $x_i$ or $\neg x_i$, so its measure is $1$, equal to its leaf count. If the root is an AND gate with subformulae computing $g,h$, then

$$
\mu(g\wedge h)\leq\mu(g)+\mu(h)
$$

by property 2; the induction hypothesis bounds this by the sum of the two subformula sizes, which is the size of $F$. Property 3 gives the identical argument for an OR gate. Consequently every formula computing $f$ has size at least $\mu(f)$, so $\mu(f)$ is a formula-size lower bound.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
