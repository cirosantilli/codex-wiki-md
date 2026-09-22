<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The same [Maxwell equations](../../../../../../maxwell-equations-split.md) give

$$
\partial_t\mathbf u^B=\frac12\nabla\times\partial_t\mathbf B
=-\frac12\nabla\times(\nabla\times\mathbf E)=\frac12\nabla^2\mathbf E,
$$

where the last equality uses $\nabla\cdot\mathbf E=0$. Combining with part (ii),

$$
\partial_t(u_i^E+u_i^B)=\frac12\nabla^2E_i-\frac{c^2}{2}\nabla^2B_i.
$$

The divergences of the symmetric gradients satisfy

$$
\partial_jS^E_{ij}=\frac12(\partial_i\partial_jE_j+\partial_j\partial_jE_i)=\frac12\nabla^2E_i,
\qquad \partial_jS^B_{ij}=\frac12\nabla^2B_i.
$$

Thus the local identity is $\partial_t(u_i^E+u_i^B)=\partial_j(S^E_{ij}-c^2S^B_{ij})$. Integrate over the fixed volume and apply the [divergence theorem](../../../../../../divergence-theorem.md) componentwise:

$$
\boxed{\frac\partial{\partial t}\int_V(u_i^E+u_i^B)\,dV
=\oint_A(S^E_{ij}-c^2S^B_{ij})\,dA_j}.
$$

Here $dA_j=n_jdA$ uses the outward [normal vector](../../../../../../normal-vector.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
