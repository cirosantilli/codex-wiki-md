<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

After the pressure enforces incompressibility, let $L$ denote the displayed linear operator. Integration by parts gives

$$
\langle\Phi_i,L\Phi_j\rangle
=-\sigma\int_V\nabla\mathbf u_i:\nabla\mathbf u_j\,dV
-\sigma\operatorname{Ra}\int_V\nabla\theta_i\mathbin\cdot\nabla\theta_j\,dV
+\sigma\operatorname{Ra}\int_V(w_i\theta_j+\theta_iw_j)\,dV.
$$

The pressure terms vanish by incompressibility and the boundary conditions. The expression is symmetric under $i\leftrightarrow j$, so

$$
\boxed{\langle\Phi_i,L\Phi_j\rangle
=\langle L\Phi_i,\Phi_j\rangle}.
$$

**Thus $L$ is a [self-adjoint operator](../../../../../../../self-adjoint-operator.md) in the energy inner product and hence a [normal operator](../../../../../../../normal-operator.md). Its orthogonal eigenmodes cannot generate non-normal transient growth.**

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
