<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the local momentum equation in the current volume:

$$
\sigma_{jk,k}=\rho(a_j-b_j).
$$

Symmetry of the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) and the product rule give

$$
\partial_k(x_i\sigma_{jk})=\sigma_{ij}+\rho x_i(a_j-b_j).
$$

Apply the [divergence theorem](../../../../../divergence-theorem.md) and use $t_j=\sigma_{jk}n_k$. The [mean stress and strain boundary identities](../../../../../mean-stress-and-strain-boundary-identities.md) follow:

$$
\boxed{V\overline\sigma_{ij}=\int_Sx_it_j\,dS+\int_V\rho x_i(b_j-a_j)\,dV.}
$$

For [infinitesimal strain tensor](../../../../../infinitesimal-strain-tensor.md), $e_{ij}=(u_{i,j}+u_{j,i})/2$, and a second application of the [divergence theorem](../../../../../divergence-theorem.md) gives

$$
\boxed{V\overline e_{ij}=\frac12\int_S(u_in_j+u_jn_i)\,dS.}
$$

To first order, evaluate self-gravity in the undeformed uniform sphere. The [shell theorem](../../../../../spherical-shell-theorem.md) says that only the enclosed mass $M(r)=4\pi\rho r^3/3$ contributes to the inward field. Consequently

$$
b(x)=-\frac{GM(r)}{r^2}\frac{x}{r}
=-\frac{4\pi G\rho}{3}x=-\frac ga x,\qquad
g=\frac{4\pi G\rho a}{3}.
$$

The field vanishes at the centre and increases linearly to its surface value.

The requested radius change concerns the final traction-free [static elastic equilibrium](../../../../../static-elastic-equilibrium.md), not the [acceleration](../../../../../acceleration.md) immediately after gravity is switched on. In equilibrium the boundary [traction](../../../../../traction.md) and [acceleration](../../../../../acceleration.md) vanish. Spherical symmetry gives

$$
\frac1V\int_Vx_ix_j\,dV=\frac{a^2}{5}\delta_{ij},\qquad
\overline\sigma_{ij}=-\frac{\rho ga}{5}\delta_{ij}.
$$

The homogeneous [linear elasticity](../../../../../linear-elasticity.md) law commutes with volume averaging:

$$
\overline\sigma=\kappa\,\operatorname{tr}(\overline e)I+
2\mu\left(\overline e-\frac13\operatorname{tr}(\overline e)I\right),
\qquad \kappa=\lambda+\frac23\mu.
$$

Thus $\overline e=e_0I$ with $e_0=-\rho ga/(15\kappa)$. This conclusion is about the mean [strain](../../../../../strain.md), not a claim that the local [strain](../../../../../strain.md) is uniform.

Let the boundary displacement be $u(a)=u_a n$. Since $\int_Sn_in_j\,dS=(4\pi a^2/3)\delta_{ij}$, the boundary identity gives $\overline e=(u_a/a)I$. Therefore the [equilibrium contraction of a self-gravitating elastic sphere](../../../../../equilibrium-contraction-of-a-self-gravitating-elastic-sphere.md) is

$$
\boxed{u_a=-\frac{\rho ga^2}{15\kappa},\qquad
\text{radius decrease}=\frac{\rho ga^2}{15\kappa}.}
$$

The [shear modulus](../../../../../shear-modulus.md) cancels because the mean deformation is purely volumetric.

The full radial field provides a useful check without assuming uniform deformation. For $u=f(r)e_r$, momentum balance is

$$
(\lambda+2\mu)\left(f''+\frac{2f'}r-\frac{2f}{r^2}\right)=\frac{\rho g}{a}r.
$$

Regularity at the centre gives $f=Ar+Br^3$, with

$$
B=\frac{\rho g}{10a(\lambda+2\mu)},\qquad
A=-\frac{5\lambda+6\mu}{3\lambda+2\mu}Ba^2
$$

from $\sigma_{rr}(a)=0$. Substitution reproduces $f(a)=-\rho ga^2/(15\kappa)$. During the transient, the [acceleration](../../../../../acceleration.md) term in the mean-stress identity remains; gravitational feedback from the small density and shape changes is higher order in the equilibrium calculation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
