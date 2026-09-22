<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For a [group homomorphism](../../../../../../group-homomorphism.md) $h:A\to B$, the dual morphism $\widehat h:\widehat B\to\widehat A$ is pullback of algebraically trivial [line bundles](../../../../../../line-bundle.md). Translations satisfy $h\circ T_x=T_{h(x)}\circ h$, and therefore

$$
\phi_{h^*L}(x)=h^*(T_{h(x)}^*L\otimes L^{-1})=(\widehat h\circ\phi_L\circ h)(x).
$$

Also $\phi_{L\otimes M}=\phi_L+\phi_M$ and $\phi_{L^{-1}}=-\phi_L$. Dualizing is additive: $\widehat{f+g}=\widehat f+\widehat g$, since algebraically trivial [line bundles](../../../../../../line-bundle.md) obey the [Theorem of the square](../../../../../../theorem-of-the-square.md). Apply these identities to the three factors defining $D_L$. The two diagonal terms cancel in the expansion

$$
\begin{aligned}
\phi_{D_L(f,g)}&=(\widehat f+\widehat g)\phi_L(f+g)-\widehat f\phi_Lf-\widehat g\phi_Lg\\
&=\widehat f\phi_Lg+\widehat g\phi_Lf.
\end{aligned}
$$

**Hence $\boxed{\phi_{D_L(f,g)}=\widehat f\circ\phi_L\circ g+\widehat g\circ\phi_L\circ f}$.**

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
