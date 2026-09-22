<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $\mathbf k=(k_x,0,k_z)\ne0$. [Incompressibility](../../../../../../incompressible-flow.md) gives $(\mathbf k\cdot\tilde{\mathbf u})f'(\xi)e^{st}=0$. Since $f$ is nonconstant and differentiable, it follows that $\mathbf k\cdot\tilde{\mathbf u}=0$; therefore

$$
\boxed{\mathbf u'\cdot\nabla\mathbf u'=e^{2st}ff'(\tilde{\mathbf u}\cdot\mathbf k)\tilde{\mathbf u}=0.}
$$

The background has no [advection](../../../../../../advection.md) of a $y$-independent perturbation. Its only remaining cross-advection term is $(\mathbf u'\cdot\nabla)\mathbf U=(-3\Omega u'_x/2+q\Omega u'_z)\mathbf e_y$. The velocity/time terms have spatial factor $f$, while $\nabla P'=\tilde P\mathbf k g'(\xi)e^{st}$. For nonzero [pressure](../../../../../../pressure.md) amplitude, $g'$ must therefore be a constant multiple of $f$; absorbing that multiple into $\tilde P$ gives $g'=f$. An additive spatial constant in $g$ is a [pressure](../../../../../../pressure.md) gauge. If $\tilde P=0$, there is no such restriction on the unused [pressure](../../../../../../pressure.md) profile.

Matching coefficients gives

$$
\boxed{\begin{aligned}
s\tilde u_x&=-k_x\tilde P/\rho_0+2\Omega\tilde u_y,\\
s\tilde u_y&=-\Omega\tilde u_x/2-q\Omega\tilde u_z,\\
s\tilde u_z&=-k_z\tilde P/\rho_0,\\
k_x\tilde u_x+k_z\tilde u_z&=0.
\end{aligned}}
$$

Because the quadratic perturbation term vanishes identically, these amplitudes give an [exact single-phase incompressible perturbation of a shear flow](../../../../../../exact-single-phase-incompressible-perturbation-of-a-shear-flow.md), not merely a first-order truncation. Any sufficiently differentiable profile with $g'=f$ works locally; boundary conditions may restrict the profiles in a particular domain.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
