<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\mathbf t=\boldsymbol\theta$. The [product rule](../../../../../../product-rule.md) applied to $Q_{ij}=\lambda(t_it_j-\delta_{ij}/2)$ gives

$$
(\nabla\cdot Q)_j=[(\nabla\lambda)\cdot\mathbf t]t_j+\lambda(\nabla\cdot\mathbf t)t_j+\lambda[(\mathbf t\cdot\nabla)\mathbf t]_j-\frac12\partial_j\lambda.
$$

Since $\operatorname{Tr}Q^2=\lambda^2/2$, substituting this vector into the divergence elastic term proves the requested form of the local density. For the radial amplitude and tangential director, the [polar coordinates](../../../../../../polar-coordinates.md) identities are

$$
\nabla\lambda=\lambda'(r)\mathbf e_r,\qquad (\nabla\lambda)\cdot\mathbf t=0,\qquad \nabla\cdot\mathbf t=0,\qquad (\mathbf t\cdot\nabla)\mathbf t=-\frac{\mathbf e_r}{r}.
$$

Hence the [tangential integer nematic defect core](../../../../../../tangential-integer-nematic-defect-core.md) has

$$
\boxed{\nabla\cdot Q=-\left(\frac{\lambda'}2+\frac\lambda r\right)\mathbf e_r,\qquad f=\frac a2\lambda^2+\frac b4\lambda^4+\frac K2\left(\frac{\lambda'}2+\frac\lambda r\right)^2.}
$$

The $1/r$ director-curvature term survives when the amplitude is constant. Replacing the divergence norm by a full tensor-gradient norm would not give this expression; it is the PDF's divergence convention that is being evaluated.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
