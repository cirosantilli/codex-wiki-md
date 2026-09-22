<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $M_{ijkl}=\int_Vx_ix_jx_kx_l\,d^3x$. It is an [isotropic tensor](../../../../../../isotropic-tensor.md) and is invariant under every permutation of its four indices. Thus the three coefficients in the general rank-four isotropic form must coincide:

$$
M_{ijkl}=C(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).
$$

A double [tensor contraction](../../../../../../tensor-contraction.md) gives

$$
15C=M_{iijj}=\int_Vr^4\,d^3x
=4\pi\int_{R_1}^{R_2}r^6\,dr
=\frac{4\pi}{7}(R_2^7-R_1^7).
$$

Here the three contracted [Kronecker delta](../../../../../../kronecker-delta.md) products contribute $9$, $3$ and $3$. Contracting instead with the four unit [vectors](../../../../../../vector.md) yields

$$
\boxed{\begin{aligned}
&\int_V\prod_{a=1}^4(\mathbf x\cdot\mathbf n_a)\,d^3x\\
&\quad=\frac{4\pi}{105}(R_2^7-R_1^7)
\big[(\mathbf n_1\cdot\mathbf n_2)(\mathbf n_3\cdot\mathbf n_4)
+(\mathbf n_1\cdot\mathbf n_3)(\mathbf n_2\cdot\mathbf n_4)
+(\mathbf n_1\cdot\mathbf n_4)(\mathbf n_2\cdot\mathbf n_3)\big].
\end{aligned}}
$$

This agrees with subtracting two instances of the [isotropic fourth moment of a ball](../../../../../../isotropic-fourth-moment-of-a-ball.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
