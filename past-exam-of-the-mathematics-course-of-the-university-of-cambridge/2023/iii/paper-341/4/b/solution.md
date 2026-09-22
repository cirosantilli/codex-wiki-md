<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [semidiscrete system](../../../../../../method-of-lines.md) as $\mathbf u'=L_h\mathbf u+\alpha D_h\mathbf u$. With zero boundary values, the centered second-difference matrix $L_h$ is symmetric negative definite and the centered first-difference matrix $D_h$ is [skew-symmetric](../../../../../../skew-symmetric-matrix.md). Therefore

$$
\frac12\frac d{dt}\|\mathbf u(t)\|_2^2
=\mathbf u^TL_h\mathbf u+\alpha\mathbf u^TD_h\mathbf u
=\mathbf u^TL_h\mathbf u\leq0.
$$

This is a mesh-uniform stability estimate for the [centered convection-diffusion semidiscretization](../../../../../../centered-convection-diffusion-semidiscretization.md), valid for every real $\alpha$.

Both centered differences have local spatial error $O(h^2)$ for a sufficiently smooth solution. Stability plus consistency gives convergence, equivalently by the semidiscrete form of the [Lax equivalence theorem](../../../../../../lax-equivalence-theorem.md). Thus

$$
\boxed{\text{the semidiscretization converges with spatial order two for every fixed }\alpha\in\mathbb R.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
