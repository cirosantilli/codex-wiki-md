<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For large $r=|\mathbf r|$, the outgoing kernel has

$$
G_k(\mathbf r,\mathbf r')=\frac{e^{ikr}}{4\pi r}e^{-ik\widehat{\mathbf r}\cdot\mathbf r'}+O(r^{-2}),\qquad \partial_{n'}G_k=-ik(\widehat{\mathbf r}\cdot\mathbf n')\frac{e^{ikr}}{4\pi r}e^{-ik\widehat{\mathbf r}\cdot\mathbf r'}+O(r^{-2}).
$$

Thus the [surface representation of an obstacle far-field pattern](../../../../../../surface-representation-of-an-obstacle-far-field-pattern.md), with $\psi_s=e^{ikr}f_\infty/r+O(r^{-2})$, gives

$$
\boxed{f_\infty(\widehat{\mathbf r},\widehat{\mathbf r}_0,k)=-\frac1{4\pi}\int_{\partial D}e^{-ik\widehat{\mathbf r}\cdot\mathbf r'}[\partial_{n'}\psi_s+ik(\widehat{\mathbf r}\cdot\mathbf n')\psi_s]\,dS'.}
$$

Conjugating the [Herglotz wave function](../../../../../../herglotz-wave-function.md) gives $\overline{v_g}(\mathbf r')=\int_{S^2}e^{-ik\widehat{\mathbf r}\cdot\mathbf r'}\overline{g(\widehat{\mathbf r})}\,dS$. Interchanging the angular and obstacle-surface integrals yields the [Herglotz pairing with an obstacle far field](../../../../../../herglotz-pairing-with-an-obstacle-far-field.md):

$$
\boxed{\int_{S^2}f_\infty(\widehat{\mathbf r},\widehat{\mathbf r}_0,k)\overline{g(\widehat{\mathbf r})}\,dS=\frac1{4\pi}\int_{\partial D}[\psi_s\partial_{n'}\overline{v_g}-\overline{v_g}\partial_{n'}\psi_s]\,dS'.}
$$

This contains only the scattered-field boundary traces and the Herglotz function, with the outward-obstacle normal convention fixing the sign.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
