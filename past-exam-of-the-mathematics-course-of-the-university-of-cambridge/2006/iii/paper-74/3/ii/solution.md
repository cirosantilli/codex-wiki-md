<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $a_h^2=k^2+m^2>0$ and $\Lambda=a_h^2+\pi^2$. The plane-layer [poloidal-toroidal decomposition](../../../../../../poloidal-toroidal-decomposition.md) supplies the assumed poloidal fields as

$$
\mathbf u=\nabla\times\nabla\times(\phi\hat{\mathbf z}),\qquad
\mathbf b=\nabla\times\nabla\times(\chi\hat{\mathbf z}).
$$

Since $w=-\Delta_h\phi$ and $b_z=-\Delta_h\chi$, potentials proportional to $e^{st+ikx+imy}\sin\pi z$ have the required vertical components. Their horizontal components are proportional to $\cos\pi z$, satisfying the [stress-free boundary conditions](../../../../../../stress-free-boundary-condition.md) and the horizontal-field [boundary conditions](../../../../../../boundary-condition.md). The double-[curl](../../../../../../curl.md) representation automatically enforces [incompressibility](../../../../../../incompressible-flow.md) and the [solenoidal magnetic-field constraint](../../../../../../solenoidal-magnetic-field-constraint.md).

Let $W,\Theta,C$ be the amplitudes of $w,\theta,b_z$. The temperature and [resistive induction equations](../../../../../../resistive-induction-equation.md) immediately give

$$
(s+\Lambda)\Theta=W,\qquad (s+\zeta\Lambda)C=imW.
$$

Eliminate the total-pressure perturbation by applying $\Delta$ to the vertical momentum equation and subtracting $\partial_z$ times its [divergence](../../../../../../divergence.md). The resulting vertical equation is

$$
\Lambda(s/\sigma+\Lambda)W=Ra_h^2\Theta+\zeta Q\,im\Lambda C.
$$

In particular, $imC=-m^2W/(s+\zeta\Lambda)$ shows explicitly that [magnetic tension](../../../../../../magnetic-tension.md) opposes the displacement.

Taking the [determinant](../../../../../../determinant.md) of these three amplitude equations gives the [horizontal-field magnetoconvection dispersion relation](../../../../../../horizontal-field-magnetoconvection-dispersion-relation.md):

$$
\boxed{\Lambda(s+\Lambda)\left[(s+\sigma\Lambda)(s+\zeta\Lambda)+\sigma\zeta Qm^2\right]
-\sigma Ra_h^2(s+\zeta\Lambda)=0.}
$$

This cubic [polynomial](../../../../../../polynomial-split.md) includes all roots of the assumed poloidal coupled system; using its determinant form avoids discarding possible roots by dividing by $s+\Lambda$ or $s+\zeta\Lambda$. As a check, $Qm^2=0$ factors off magnetic diffusion and leaves the standard stress-free [Rayleigh-Bénard convection](../../../../../../rayleigh-benard-convection.md) growth equation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
