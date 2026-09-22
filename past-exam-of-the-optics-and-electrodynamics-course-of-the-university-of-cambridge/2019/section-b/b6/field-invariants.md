<h1 id="section-b/b6/field-invariants">Field invariants</h1>

↑ **Parent:** [Solution](solution.md)

Let $\mathbf u$ be the boost [velocity](../../../../velocity.md), and decompose the fields into components parallel and perpendicular to it. The parallel components are unchanged. The perpendicular components obey

$$
\mathbf E'_\perp=\gamma(\mathbf E_\perp+\mathbf u\times\mathbf B_\perp),\qquad
\mathbf B'_\perp=\gamma(\mathbf B_\perp-\mathbf u\times\mathbf E_\perp/c^2),\qquad
\gamma=(1-u^2/c^2)^{-1/2}.
$$

All vectors inside these expressions are perpendicular to $\mathbf u$. Thus $|\mathbf u\times\mathbf B_\perp|^2=u^2B_\perp^2$, and similarly for $\mathbf E_\perp$. In the difference of squares, the mixed terms cancel because

$$
\mathbf E_\perp\cdot(\mathbf u\times\mathbf B_\perp)
=-\mathbf B_\perp\cdot(\mathbf u\times\mathbf E_\perp).
$$

It follows that

$$
\begin{aligned}
E_\perp'^2-c^2B_\perp'^2
&=\gamma^2\left[(1-u^2/c^2)E_\perp^2-(c^2-u^2)B_\perp^2\right]\\
&=E_\perp^2-c^2B_\perp^2.
\end{aligned}
$$

Adding the unchanged parallel components proves

$$
\boxed{E'^2-c^2B'^2=E^2-c^2B^2.}
$$

For the mixed [dot product](../../../../dot-product.md), expand directly. The terms $\mathbf E_\perp\cdot(\mathbf u\times\mathbf E_\perp)$ and $(\mathbf u\times\mathbf B_\perp)\cdot\mathbf B_\perp$ vanish. The remaining cross-product identity is

$$
(\mathbf u\times\mathbf B_\perp)\cdot(\mathbf u\times\mathbf E_\perp)
=u^2\mathbf E_\perp\cdot\mathbf B_\perp.
$$

Hence

$$
\mathbf E'_\perp\cdot\mathbf B'_\perp
=\gamma^2(1-u^2/c^2)\mathbf E_\perp\cdot\mathbf B_\perp
=\mathbf E_\perp\cdot\mathbf B_\perp.
$$

Parallel-perpendicular mixed [dot products](../../../../dot-product.md) are zero in both frames, so

$$
\boxed{\mathbf E'\cdot\mathbf B'=\mathbf E\cdot\mathbf B.}
$$

Rotations also preserve these two expressions, completing the proof for proper [Lorentz transformations](../../../../lorentz-transformation.md). The second expression is a pseudoscalar under spatial parity, but is invariant under the boosts at issue here.

These results also follow from [tensor contractions](../../../../tensor-contraction.md). In the convention used below, $F_{\mu\nu}F^{\mu\nu}=2(B^2-E^2/c^2)$ and $F_{\mu\nu}\widetilde F^{\mu\nu}=-4\mathbf E\cdot\mathbf B/c$. The numerical sign of the latter depends on the chosen orientation of the [dual electromagnetic field tensor](../../../../dual-electromagnetic-field-tensor.md), while its invariance under proper [Lorentz transformations](../../../../lorentz-transformation.md) does not.

## ↑ Ancestors (14)

1. [Solution](solution.md)
2. [B6](../b6.md)
3. [Section B](../../section-b.md)
4. [2019](../../../2019-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
