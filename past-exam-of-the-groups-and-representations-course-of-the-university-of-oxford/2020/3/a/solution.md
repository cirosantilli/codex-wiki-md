<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The componentwise product is closed in $G_1\times G_2$. Associativity follows componentwise from associativity in each [group](../../../../group-split.md):

$$
((g_1,g_2)(h_1,h_2))(k_1,k_2)
=((g_1h_1)k_1,(g_2h_2)k_2)
=(g_1(h_1k_1),g_2(h_2k_2)).
$$

The identity is $(e_1,e_2)$, and $(g_1,g_2)^{-1}=(g_1^{-1},g_2^{-1})$. These verify all the [group axioms](../../../../group-axioms.md), so this is the [direct product of groups](../../../../direct-product-of-groups.md).

Write the paper's [Kronecker product](../../../../kronecker-product.md) $\times$ as $\otimes$. Its mixed-product identity and the [representation](../../../../group-representation.md) laws of $R_1,R_2$ give

$$
\begin{aligned}
R(g_1,g_2)R(h_1,h_2)
&=(R_1(g_1)\otimes R_2(g_2))(R_1(h_1)\otimes R_2(h_2))\\
&=R_1(g_1)R_1(h_1)\otimes R_2(g_2)R_2(h_2)\\
&=R_1(g_1h_1)\otimes R_2(g_2h_2)\\
&=R((g_1,g_2)(h_1,h_2)).
\end{aligned}
$$

Also $R(e_1,e_2)=I_{n_1}\otimes I_{n_2}=I_{n_1n_2}$, and

$$
R(g_1,g_2)^{-1}=R_1(g_1)^{-1}\otimes R_2(g_2)^{-1}.
$$

Thus the images are invertible and this is a [group representation](../../../../group-representation.md) of [dimension](../../../../dimension-vector-space.md) $n_1n_2$, called the [external tensor product of group representations](../../../../external-tensor-product-of-group-representations.md). No irreducibility assumption is needed for this construction.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
