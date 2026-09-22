<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For any measurable set $A$, integrating the joint acceptance event in [rejection sampling](../../../../../../../rejection-sampling.md) gives

$$
P(Y\in A,\text{accept})=\int_Ag(y)\frac{f(y)}{Cg(y)}\,dy=\frac1C\int_Af(y)\,dy.
$$

Setting $A$ equal to the whole support yields $P(\text{accept})=1/C$. Thus

$$
\boxed{P(Y\in A\mid\text{accept})=\int_A f(y)\,dy.}
$$

To verify repeated attempts directly, the [probability](../../../../../../../probability.md) that the first accepted observation falls in $A$ is

$$
\sum_{r=1}^{\infty}(1-1/C)^{r-1}\frac1C\int_A f(y)\,dy=\int_A f(y)\,dy.
$$

With finite $C$, eventual acceptance has [probability](../../../../../../../probability.md) one. Applying the same argument after each success proves that the retained sequence consists of independent draws from the target.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
