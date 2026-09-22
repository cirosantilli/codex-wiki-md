<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The spatial factor $r^lY_l^m$ is a [regular solid harmonic](../../../../../../regular-solid-harmonic.md). Besides the [Laplace equation](../../../../../../laplace-equation.md) $\nabla^2F=0$, homogeneity gives $\mathbf r\cdot\nabla F=lF$. The divergence of the [fluid displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md) is

$$
\begin{aligned}
\nabla\cdot(UF\mathbf r)
&=[rU'+(l+3)U]F,\\
\nabla\cdot(V\nabla F)
&=\frac{l}{r}V'F.
\end{aligned}
$$

Define the scalar dilation amplitude $D_r=rU'+(l+3)U+(l/r)V'$; this is the quantity denoted $\Delta$ in the question, not the notation $\Delta_L$ for a [Lagrangian pressure perturbation](../../../../../../lagrangian-pressure-perturbation.md). Then [mass conservation](../../../../../../mass-conservation.md) gives $\widehat\rho=-\rho D_r$.

The equilibrium pressure gradient and homogeneity identity give

$$
\boldsymbol\xi\cdot\nabla p
=-\rho\omega_d^2(Ur^2+lV)F.
$$

Consequently the [adiabatic equation of state](../../../../../../adiabatic-equation-of-state.md) yields

$$
\boxed{\widehat\rho=-\rho D_r,\qquad
\widehat p=\rho\omega_d^2(Ur^2+lV)-\gamma pD_r.}
$$

For the force equations, the product rule gives

$$
\nabla(\widehat pF)=\widehat p'F\mathbf e_r+\widehat p\nabla F,\qquad
\nabla(\widehat\Phi F)=\widehat\Phi'F\mathbf e_r+\widehat\Phi\nabla F.
$$

Equating the coefficients of $F\mathbf e_r$ and $\nabla F$ in the [self-gravitating adiabatic displacement equations](../../../../../../self-gravitating-adiabatic-displacement-equations.md) gives

$$
\boxed{\rho\omega^2Ur
=\widehat\rho\,\omega_d^2r+\rho\widehat\Phi'+\widehat p',
\qquad
\rho\omega^2V=\rho\widehat\Phi+\widehat p.}
$$

Finally, applying the [Laplacian](../../../../../../laplacian.md) to the gravitational perturbation gives

$$
\nabla^2(\widehat\Phi F)
=\left(\widehat\Phi''+\frac{2(l+1)}r\widehat\Phi'\right)F,
$$

so the [Poisson equation](../../../../../../poisson-equation.md) becomes

$$
\boxed{\widehat\Phi''+\frac{2(l+1)}r\widehat\Phi'
=4\pi G\,\widehat\rho,\qquad
D_r=rU'+(l+3)U+\frac lrV'.}
$$

These are the required interior equations for [uniform-density stellar oscillation](../../../../../../uniform-density-stellar-oscillation.md).

There is a radial degeneracy at $l=0$: $F$ is spatially constant and $\nabla F=0$, so the displacement is independent of $V$. The second force equation then cannot be inferred by equating independent vectors. For nonzero $\omega$ it may be imposed as an auxiliary definition of $V$, but it is not an additional physical radial equation. At zero frequency the radial equations should be used directly. This distinction matters for interpreting the zero factor in (c).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
