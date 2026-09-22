<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [rotational invariance of a central-potential Hamiltonian](../../../../../../../rotational-invariance-of-a-central-potential-hamiltonian.md) allows a simultaneous [eigenstate](../../../../../../../eigenstate.md) of energy and the two-dimensional [orbital angular momentum](../../../../../../../orbital-angular-momentum.md) $L_z=-i\hbar\partial_\phi$. For a separated [wavefunction](../../../../../../../wave-function.md) $F(r)G(\phi)$, the [Laplacian in polar coordinates](../../../../../../../laplacian-in-polar-coordinates.md) gives

$$
\frac{r^2}{F}\left(F''+\frac1rF'\right)+\frac{G''}{G}+\frac{2m r^2}{\hbar^2}(E-V)=0.
$$

The $\phi$ term must be a constant; write $G''/G=-k^2$. The angular [eigenfunctions](../../../../../../../eigenfunction.md) can be chosen as $e^{ik\phi}$. Single-valuedness under $\phi\mapsto\phi+2\pi$ imposes $e^{2\pi i k}=1$, hence $k\in\mathbb Z$. The radial equation in the [separation of a two-dimensional central-potential eigenstate](../../../../../../../separation-of-a-two-dimensional-central-potential-eigenstate.md) is

$$
-\frac{\hbar^2}{2m}\left(f''+\frac1rf'-\frac{k^2}{r^2}f\right)+V(r)f=Ef.
$$

For a real [central potential](../../../../../../../central-potential.md) and the usual real self-adjoint radial boundary conditions, the radial equation admits a basis of real solutions: real and imaginary parts of a complex solution obey the same equation and boundary conditions. Choose a real normalized radial [eigenfunction](../../../../../../../eigenfunction.md). Since the plane area element in [plane polar coordinates](../../../../../../../plane-polar-coordinates.md) is $r\,dr\,d\phi$, the normalization is

$$
\int_0^\infty r f(r)^2\,dr=1,\qquad
\boxed{\psi_k(r,\phi)=\frac{f(r)}{\sqrt{2\pi}}e^{ik\phi},\quad k\in\mathbb Z}.
$$

This establishes the intended separated simultaneous [eigenstate](../../../../../../../eigenstate.md) form. **It is not the form of every stationary state.** The radial equation depends on $k^2$, so the $k$ and $-k$ sectors have the same energy. For $k\geq1$, their normalized superposition

$$
\psi_{\rm real}(r,\phi)=\frac{f(r)}{\sqrt\pi}\cos(k\phi)
$$

is a single-valued [stationary state](../../../../../../../stationary-state.md) with that energy but is not a single angular exponential. [Quantum degeneracy](../../../../../../../degenerate-energy-levels.md) is precisely why [separation of variables](../../../../../../../separation-of-variables.md) selects a convenient [eigenstate](../../../../../../../eigenstate.md) basis rather than all vectors in an energy eigenspace. The printed assertion needs this qualification. The printed polar-coordinate aid also labels a gradient component tuple as a divergence; the [gradient](../../../../../../../gradient.md) used below is the two-dimensional vector $\widehat{\mathbf r}\partial_r+\widehat{\boldsymbol\phi}r^{-1}\partial_\phi$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
