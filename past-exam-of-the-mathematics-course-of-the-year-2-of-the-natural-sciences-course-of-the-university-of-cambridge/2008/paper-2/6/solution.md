<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Under an orthogonal change of [Cartesian coordinates](../../../../cartesian-coordinate-system.md) with $x_i'=R_{ia}x_a$, a rank-$n$ [Cartesian tensor](../../../../cartesian-tensor.md) transforms as $T'_{i_1\cdots i_n}=R_{i_1j_1}\cdots R_{i_nj_n}T_{j_1\cdots j_n}$, summing repeated indices. An [isotropic tensor](../../../../isotropic-tensor.md) is invariant under every rotation. For an [isotropic fourth-rank tensor](../../../../isotropic-fourth-rank-tensor.md), half-turns about the coordinate axes eliminate components unless each coordinate label occurs an even number of times. Coordinate rotations make the remaining two-pair patterns depend on three constants $c_{1122}=\alpha$, $c_{1212}=\beta$, $c_{1221}=\gamma$. Invariance after rotating the first axis to $(e_1+e_2)/\sqrt2$ gives $c_{1111}=\alpha+\beta+\gamma$. Hence

$$
c_{ijkl}=\alpha\delta_{ij}\delta_{kl}+\beta\delta_{ik}\delta_{jl}+\gamma\delta_{il}\delta_{jk}.
$$

This is a direct proof of the rank-four isotropic decomposition, without assuming any prior interchange symmetry of the four indices. Each displayed delta pairing is itself rotation invariant.

For symmetric [strain](../../../../strain.md), contraction gives $\sigma_{ij}=\alpha e_{kk}\delta_{ij}+(\beta+\gamma)e_{ij}$. Comparing with the [Lamé parameters](../../../../lame-parameter.md) yields

$$
\boxed{\lambda=\alpha,\qquad\mu=\frac{\beta+\gamma}2.}
$$

Write $p=e_{kk}/3$ and $d_{ij}=e_{ij}-p\delta_{ij}$, so $d_{kk}=0$. Since $e_{ij}e_{ij}=3p^2+d_{ij}d_{ij}$, the [strain energy density](../../../../strain-energy-density.md) becomes

$$
E=\frac\lambda2(e_{kk})^2+\mu e_{ij}e_{ij}
=\frac12\left(\lambda+\frac{2\mu}3\right)(e_{kk})^2+\mu d_{ij}d_{ij}.
$$

The two terms describe volumetric and shear deformation, respectively. Thus [nonnegative isotropic elastic strain energy](../../../../nonnegative-isotropic-elastic-strain-energy.md) is equivalent to

$$
\boxed{\mu\geq0,\qquad\lambda\geq-\frac{2\mu}3.}
$$

Necessity also follows by taking a nonzero traceless [strain](../../../../strain.md) and a pure dilation separately. The combination $K=\lambda+2\mu/3$ is the [bulk modulus](../../../../bulk-modulus.md); strict inequalities give positive energy for every nonzero [strain](../../../../strain.md).

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
