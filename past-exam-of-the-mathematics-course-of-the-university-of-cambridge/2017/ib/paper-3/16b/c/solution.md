<h1 id="16b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the radial exponential $e^{-\alpha r}$ shown in the original PDF; the TeX's $e^{-\alpha x}$ is a transcription defect. Every orbital [angular momentum operator](../../../../../../angular-momentum-operator.md) annihilates a radial function, so it acts only on $P=x_1+x_2+2x_3$. The [angular momentum of a radial function times a linear polynomial](../../../../../../angular-momentum-of-a-radial-function-times-a-linear-polynomial.md) is determined by its degree-one angular factor: direct application of the rotation derivatives gives

$$
\hat L^2P=2\hbar^2P.
$$

Equivalently its restriction to the sphere is a degree-one [spherical harmonic](../../../../../../spherical-harmonic.md). Thus

$$
\boxed{\hat L^2\psi=2\hbar^2\psi,\qquad l(l+1)=2,\quad l=1.}
$$

Furthermore $\hat L_3\psi=-i\hbar K(x_1-x_2)e^{-\alpha r}$. Its [expected value](../../../../../../expected-value.md) is proportional to the integral of $(x_1+x_2+2x_3)(x_1-x_2)e^{-2\alpha r}$. The cross terms are odd in a coordinate, and the integrals of $x_1^2$ and $x_2^2$ agree by rotational symmetry. Hence

$$
\boxed{\langle\hat L_3\rangle_\psi=0.}
$$

The state need not be an eigenstate of $\hat L_3$. If normalization is desired, $\int P^2e^{-2\alpha r}\,d^3x=6\pi/\alpha^5$, so $K=\alpha^{5/2}/\sqrt{6\pi}$; the zero expectation holds after normalization for any nonzero initial $K$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16B](../../16b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
