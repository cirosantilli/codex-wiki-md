<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is

$$
\boxed{K=\{g\in G:\Phi(g)=e_{G'}\}.}
$$

The homomorphism sends identity to identity and inverses to inverses. Thus $e_G\in K$, and if $k_1,k_2\in K$, then $\Phi(k_1k_2^{-1})=e_{G'}$, so $K$ is a subgroup by the [subgroup test](../../../../../subgroup-test.md).

For any $g\in G$ and $k\in K$,

$$
\Phi(gkg^{-1})=\Phi(g)\Phi(k)\Phi(g)^{-1}=\Phi(g)e_{G'}\Phi(g)^{-1}=e_{G'}.
$$

Hence $gKg^{-1}\subseteq K$. Applying the same inclusion with $g^{-1}$ gives equality, proving

$$
\boxed{K\trianglelefteq G.}
$$

This normality argument does not require either group to be finite.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
