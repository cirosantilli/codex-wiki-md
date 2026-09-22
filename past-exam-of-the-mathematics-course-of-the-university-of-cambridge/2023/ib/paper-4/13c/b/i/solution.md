<h1 id="13c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [displacement gradient tensor](../../../../../../../displacement-gradient-tensor.md) specified in the question,

$$
\nabla\mathbf u:\nabla\mathbf u^T
=\operatorname{tr}(\nabla\mathbf u\,\nabla\mathbf u^T)
=u_x^2+u_y^2+v_x^2+v_y^2,
$$

while the [divergence](../../../../../../../divergence.md) is $\nabla\cdot\mathbf u=u_x+v_y$. Hence the [isotropic linear-elastic energy density](../../../../../../../isotropic-linear-elastic-energy-density.md) is

$$
\frac\mu2(u_x^2+u_y^2+v_x^2+v_y^2)
+\frac{\lambda+\mu}{2}(u_x+v_y)^2.
$$

Expanding the square and collecting terms yields

$$
\boxed{
\mathcal J=\iint_\Omega\left[
\left(\frac\lambda2+\mu\right)(u_x^2+v_y^2)
+\frac\mu2(u_y^2+v_x^2)
+(\lambda+\mu)u_xv_y
\right]dx\,dy}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [13C](../../../13c.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
