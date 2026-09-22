<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The fixed-displacement [boundary value problem](../../../../../../boundary-value-problem.md) now has $u=0$ on the whole boundary. The [elastic normal-mode energy identity](../../../../../../elastic-normal-mode-energy-identity.md) still holds, because its boundary term contains $\overline u$. Define

$$
B_{\alpha i\beta j}=K_{k\gamma}\epsilon_{\alpha\beta\gamma}\epsilon_{ijk},\qquad H_{\alpha i\beta j}=c_{\alpha i\beta j}+B_{\alpha i\beta j}.
$$

For real constant $K$, $B$ has major symmetry: both [Levi-Civita symbols](../../../../../../levi-civita-symbol.md) change sign upon exchanging the two index pairs. Its quadratic density is a [quadratic minor null Lagrangian](../../../../../../quadratic-minor-null-lagrangian.md). Indeed,

$$
\begin{aligned}
\int_{\Omega_0}\overline{u_{i,\alpha}}B_{\alpha i\beta j}u_{j,\beta}\,dV
&=\int_{\partial\Omega_0}\nu_\alpha\overline{u_i}B_{\alpha i\beta j}u_{j,\beta}\,dS\\
&\quad-\int_{\Omega_0}\overline{u_i}K_{k\gamma}\epsilon_{\alpha\beta\gamma}\epsilon_{ijk}u_{j,\beta\alpha}\,dV=0.
\end{aligned}
$$

The boundary integral vanishes by the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md), and the volume integral vanishes because mixed derivatives are symmetric in $\alpha,\beta$ whereas $\epsilon_{\alpha\beta\gamma}$ is antisymmetric. Constancy of $K$ is essential: otherwise its derivatives would produce extra terms. This calculation initially applies to smooth fields and extends to fields with zero Sobolev boundary trace by density.

It follows that the [Rayleigh quotient](../../../../../../rayleigh-quotient.md) numerator can be replaced by the quadratic form with $H$:

$$
\omega^2\int_{\Omega_0}\rho_0|u|^2\,dV=\int_{\Omega_0}\overline{u_{i,\alpha}}H_{\alpha i\beta j}u_{j,\beta}\,dV.
$$

The assumed positivity of $H$ on all nonzero real matrices also gives positivity on nonzero complex matrices by splitting real and imaginary parts. A nonzero $u$ satisfying $u=0$ on the boundary cannot have identically zero gradient. Hence the right side is strictly positive, and

$$
\boxed{\omega^2>0\quad\text{for every nonzero fixed-boundary mode}.}
$$

This works even when the original moduli quadratic form is not pointwise positive on all matrices: its integrated energy on fixed-boundary gradients agrees with a positive density after adding the [quadratic minor null Lagrangian](../../../../../../quadratic-minor-null-lagrangian.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
