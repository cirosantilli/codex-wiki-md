<h1 id="36c/solution">Solution</h1>

↑ **Parent:** [36C](../36c.md)

In the [Landau-Ginzburg theory](../../../../../landau-ginzburg-theory.md) functional, $B^2/(2\mu_0)$ is the magnetic field energy density; the covariant-gradient term is the carrier kinetic energy including phase gradients and electromagnetic coupling. The terms $\alpha|\psi|^2+\beta|\psi|^4$ give the local condensation energy. With the normalization in the question, $n=|\psi|^2$ is the carrier density.

For a uniform field-free equilibrium, minimize $\alpha n+\beta n^2$ over $n\geq0$. Stability for large $n$ requires $\beta>0$, and a nonzero minimum requires $\alpha<0$. Therefore

$$
\boxed{n=-\frac\alpha{2\beta}>0.}
$$

The factor two follows from the question's quartic coefficient $\beta$, rather than a convention using $\beta/2$.

Let $D_A=-i\hbar\nabla-qA$. Under the [gauge transformation](../../../../../gauge-transformation.md),

$$
D_{A+\nabla\Lambda}(e^{iq\Lambda/\hbar}\psi)=e^{iq\Lambda/\hbar}D_A\psi.
$$

Its squared magnitude is unchanged, $|\psi|$ is unchanged, and $B=\nabla\times A$ is unchanged. Thus the full energy has [gauge invariance](../../../../../gauge-invariance.md).

For uniform $n$, write $\psi=\sqrt n\,e^{i\phi}$. The kinetic density is $n(\hbar\nabla\phi-qA)^2/(2m)$. Varying $A$ with compactly supported variations and integrating the magnetic term by parts gives

$$
\delta E=\int\left[\frac1{\mu_0}\nabla\times B+\frac{nq^2}{m}\left(A-\frac\hbar q\nabla\phi\right)\right]\cdot\delta A\,d^3x.
$$

At a minimum its coefficient vanishes, giving the [London equation](../../../../../london-equations.md)

$$
\boxed{\nabla\times B=-\frac{\mu_0q^2n}{m}\left(A-\frac\hbar q\nabla\phi\right).}
$$

Taking another curl, using $\nabla\cdot B=0$ and a smooth phase so $\nabla\times\nabla\phi=0$, yields

$$
\boxed{\nabla^2B=\frac B{\lambda_L^2},\qquad\lambda_L=\sqrt{\frac{m}{\mu_0q^2n}}.}
$$

For a planar surface this has the decaying solution $B(x)=B(0)e^{-x/\lambda_L}$ inside the material; the growing solution is excluded by boundedness in the bulk. Hence magnetic fields penetrate only a surface layer of thickness $\lambda_L$ and vanish deep in the macroscopic bulk, the [Meissner effect](../../../../../meissner-effect.md). This conclusion uses the uniform-density, smooth-phase setting; a vortex has a singular phase and a nonuniform core and is outside those assumptions.

## ↑ Ancestors (11)

1. [36C](../36c.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
