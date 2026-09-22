<h1 id="9/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [image of a group homomorphism](../../../../../image-of-a-group-homomorphism.md) contains $e_{G_2}=\phi(e_{G_1})$. If $u=\phi(g)$ and $v=\phi(h)$ lie in the image, then $uv^{-1}=\phi(gh^{-1})$ also lies there. The [subgroup test](../../../../../subgroup-test.md) proves $\operatorname{im}\phi\leq G_2$.

The [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is $K=\{g:\phi(g)=e_{G_2}\}$. It is nonempty and closed under $kh^{-1}$ for $k,h\in K$, so it is a subgroup. For any $g\in G_1$ and $k\in K$,

$$
\phi(gkg^{-1})=\phi(g)\phi(k)\phi(g)^{-1}=e_{G_2}.
$$

Thus $gKg^{-1}\subseteq K$. Replacing $g$ by $g^{-1}$ gives the reverse inclusion, proving

$$
\boxed{K\trianglelefteq G_1.}
$$

Finally, if $K=\{e\}$ and $\phi(g)=\phi(h)$, then $\phi(h^{-1}g)=e$. Thus $h^{-1}g\in K$ forces $g=h$, establishing injectivity. Conversely an injective homomorphism has trivial kernel, so

$$
\boxed{\phi\text{ injective}\quad\Longleftrightarrow\quad\ker\phi=\{e\}.}
$$

None of these arguments requires either group to be finite.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
