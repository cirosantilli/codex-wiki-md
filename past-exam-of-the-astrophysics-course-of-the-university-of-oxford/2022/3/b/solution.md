<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Insert the diagonal covariance from [a](../a.md) into the two-point function and apply the [spherical harmonic addition theorem](../../../../spherical-harmonic-addition-theorem.md):

$$
C(\alpha)=\sum_l C_l\sum_{m=-l}^l\mathcal Y_{lm}(\hat n)\mathcal Y_{lm}^*(\hat m)
=\boxed{\frac{1}{4\pi}\sum_{l=0}^\infty(2l+1)C_lP_l(\cos\alpha)}.
$$

The [Legendre polynomials](../../../../legendre-polynomial.md) encode the angular separation. Since $P_l(1)=1$, the zero-separation value $C(0)=\langle\Theta^2\rangle$ is the total [variance](../../../../variance-split.md). For measured [Cosmic microwave background anisotropy](../../../../cosmic-microwave-background-anisotropy-split.md), remove the monopole and usually the kinematic dipole, so the corresponding sum starts at $l=2$; an instrument's angular response supplies an additional window function.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
