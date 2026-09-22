<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The primary vorticity [Jacobian determinant](../../../../../../jacobian-determinant.md) vanishes because $\nabla^2\psi=-s\psi$. The quadratic [temperature](../../../../../../temperature.md) [Jacobian determinant](../../../../../../jacobian-determinant.md) is

$$
J(\psi,b\cos\alpha x\sin\pi z)=\frac{\alpha\pi ab}{2}\sin2\pi z.
$$

The mean [temperature](../../../../../../temperature.md) correction therefore obeys $\dot c=-4\pi^2c-\alpha\pi ab/2$. Its [Jacobian determinant](../../../../../../jacobian-determinant.md) with the primary [streamfunction](../../../../../../stream-function.md) is

$$
J(\psi,c\sin2\pi z)=\alpha\pi ac\cos\alpha x(\sin3\pi z-\sin\pi z).
$$

Projecting on the retained primary modes gives, with $D=s+Q\pi^2/s$,

$$
\dot a=-\sigma Da+\sigma R\alpha b/s,\quad
\dot b=-sb+\alpha a+\alpha\pi ac,\quad
\dot c=-4\pi^2c-\alpha\pi ab/2.
$$

For a nonzero steady roll, $b=(s^2+Q\pi^2)a/(R\alpha)$ and $c=-\alpha ab/(8\pi)$. Substitution in the second equation gives, within this truncation,

$$
\boxed{a^2=\frac{8(R-R_c)}{s^2+Q\pi^2},\qquad c=-\frac{R-R_c}{\pi R}.}
$$

The positive denominator ensures branches only on the supercritical side for every $Q\ge0$. To verify [dynamical stability](../../../../../../stability-theory.md) as well as existence, the critical right [eigenvector](../../../../../../eigenvector.md) is $(1,\alpha/s)$; normalizing the left [eigenvector](../../../../../../eigenvector.md) gives linear [eigenvalue](../../../../../../eigenvalue.md) derivative

$$
K=\frac{\sigma\alpha^2}{s(s+\sigma D)}>0.
$$

Quadratic slaving gives $c=-\alpha^2a^2/(8\pi s)$, and projection of its feedback gives the cubic amplitude equation

$$
\boxed{\dot a=K\left[(R-R_c)a-\frac{s^2+Q\pi^2}{8}a^3\right]+\cdots.}
$$

Its nonzero branches are stable in the center direction, while all other [eigenvalues](../../../../../../eigenvalue.md) remain negative at a simple onset. [Reflection](../../../../../../reflection-mathematics.md) about the mid-width sends $a\to-a$, so the bifurcation is **a supercritical [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) for all $Q$**, in the generic case of a single critical roll mode.

The [cubic saturation of quasistatic magnetoconvection](../../../../../../cubic-saturation-of-quasistatic-magnetoconvection.md) result is identical in [Fourier truncation](../../../../../../fourier-truncation.md) and perturbation theory at the orders needed here. At quadratic order the only forced mode is precisely the retained horizontally uniform $\sin2\pi z$ [temperature](../../../../../../temperature.md) mode. At cubic order its feedback projects on the primary mode with the same coefficient. The generated third vertical harmonic is orthogonal to that primary projection and contributes only to higher-order corrections. Thus both methods give the same linear threshold and cubic solvability condition; the truncated finite-amplitude branch is not an exact solution of the full PDE at all amplitudes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
