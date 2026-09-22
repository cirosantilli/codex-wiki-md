<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the specified affine linear [PTT fluid](../../../../../../phan-thien-tanner-fluid.md), perturb about the relaxed state $A=0$, $\mathbf v=0$. Products of $A$ with the [velocity gradient](../../../../../../velocity-gradient.md) and the term $\alpha(\operatorname{tr}A)A$ are second order in the perturbation. The material-advection term is also second order. The linearized equation is therefore

$$
\partial_t A+\frac A\tau=2E.
$$

With vanishing stress in the remote past, an [integrating factor](../../../../../../integrating-factor.md) gives

$$
A(t)=2\int_0^\infty e^{-s/\tau}E(t-s)\,ds.
$$

Since $\sigma' =G_0A$, comparison with the [linear viscoelastic fluid](../../../../../../linear-viscoelastic-fluid.md) convolution yields **$G(s)=G_0e^{-s/\tau}$** and [zero-shear viscosity](../../../../../../zero-shear-viscosity.md) $G_0\tau$. The nonlinear relaxation parameter does not appear at linear order; the response is that of a [Maxwell fluid](../../../../../../linear-maxwell-fluid.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
