<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume nonrelativistic [pressureless matter](../../../../../pressureless-matter.md), an initial [irrotational vector field](../../../../../irrotational-vector-field.md) of growing-mode [linear cosmological density perturbations](../../../../../linear-cosmological-density-perturbation-split.md), a homogeneous expanding background, and no [shell crossing](../../../../../shell-crossing.md). All gradients below refer to initial [comoving coordinates](../../../../../comoving-coordinate.md). Let $\rho_0=\bar\rho_m(t)a^3(t)=\bar\rho_m(t_i)$, with $a(t_i)=1$, and normalize the [linear growth factor](../../../../../linear-growth-factor.md) by $D(t_i)=1$. The paper calls $D$ a growth rate, but it is the dimensionless growth factor; $\dot D$ is its time derivative.

Writing $\mathbf x_i$ for the actual position at $t_i$, the [Zeldovich approximation](../../../../../zeldovich-approximation.md) is, to first order,

$$
\mathbf x(t)=\mathbf x_i+[D(t)-1]\mathbf s(\mathbf x_i),
\qquad
\dot{\mathbf x}=\dot D\,\mathbf s(\mathbf x_i).
$$

This explicitly gives $\mathbf x(t_i)=\mathbf x_i$. The usual notation $\mathbf x=\mathbf q+D\mathbf s(\mathbf q)$ instead uses the uniform reference [Lagrangian coordinate](../../../../../lagrangian-coordinate.md) $\mathbf q$, with $\mathbf x_i=\mathbf q+\mathbf s(\mathbf q)$. The two labels can be interchanged inside a first-order displacement, but not in the unperturbed position without the initial displacement correction.

To determine $\mathbf s$, [mass conservation](../../../../../mass-conservation.md) between the initial and current positions gives

$$
1+\delta(t)=\frac{1+\delta_i}{\det[\mathbf 1+(D-1)\nabla\mathbf s]}
=1+\delta_i-(D-1)\nabla\cdot\mathbf s+O(\delta_i^2).
$$

Demanding $\delta(t)=D(t)\delta_i$ gives $\nabla\cdot\mathbf s=-\delta_i$. The [irrotational vector field](../../../../../irrotational-vector-field.md) assumption makes $\mathbf s$ a gradient; the initial [cosmological Poisson equation](../../../../../cosmological-poisson-equation.md) is $\nabla^2\Phi_i=4\pi G\rho_0\delta_i$. With the same boundary conditions for these potential equations, and after removing an irrelevant uniform translation,

$$
\mathbf s=-\frac{\nabla\Phi_i}{4\pi G\rho_0},
\qquad
\boxed{\dot{\mathbf x}
=-\frac{\dot D}{4\pi G\bar\rho_m a^3}\nabla\Phi_i.}
$$

The evolution of $D$ follows from the linearized peculiar-motion equation $\ddot{\mathbf x}+2H\dot{\mathbf x}=-\nabla\Phi/a^2$. Since [cosmological Poisson equation](../../../../../cosmological-poisson-equation.md) gives $\Phi(t)=(D/a)\Phi_i$ to this order, substitution yields the [linear growth equation](../../../../../linear-growth-equation.md)

$$
\ddot D+2H\dot D-4\pi G\bar\rho_mD=0.
$$

Thus the approximation extrapolates the linear growing displacement along a fixed initial direction, even as its density mapping becomes nonlinear.

The early spin of a [dark matter halo](../../../../../dark-matter-halo.md) comes from an external gravitational [torque](../../../../../torque.md) on its nonspherical initial mass region. A uniform external acceleration moves its [centre of mass](../../../../../center-of-mass.md) without spinning it; the spatially varying [tidal tensor](../../../../../tidal-tensor.md) exerts different forces on different parts. The [tidal torque theory](../../../../../tidal-torque-theory.md) requires misalignment of the region's shape and the surrounding tidal field. A local [irrotational vector field](../../../../../irrotational-vector-field.md) of velocity does not imply zero integrated [angular momentum](../../../../../angular-momentum.md) for a nonspherical region.

Put $\mathbf y=\mathbf x_i-\hat{\mathbf x}_i$ and use the physical [peculiar velocity](../../../../../peculiar-velocity.md) $\mathbf v=a\dot{\mathbf x}$. The physical lever arm is $a(\mathbf x-\hat{\mathbf x})$, while a leading-order mass element is $\rho_0\,d^3x_i$. Substituting the velocity formula into the supplied definition of [angular momentum about the centre of mass](../../../../../angular-momentum-about-the-centre-of-mass.md) gives

$$
\mathbf J=-\frac{a^2\dot D}{4\pi G}
\int_{V_L}\mathbf y\times\nabla\Phi_i\,d^3x_i.
$$

Terms from the perturbed mass measure are higher order. Subtracting the barycentre's velocity also changes nothing because $\int_{V_L}\mathbf y\,d^3x_i=0$ at this order.

Apply the [divergence theorem](../../../../../divergence-theorem.md) componentwise:

$$
\epsilon_{jkl}\int_{V_L}y_k\partial_l\Phi_i\,d^3x_i
=\epsilon_{jkl}\int_{\Sigma_L}\Phi_i y_k\,dS_l
-\epsilon_{jkl}\int_{V_L}\Phi_i\delta_{kl}\,d^3x_i
=\epsilon_{jkl}\int_{\Sigma_L}\Phi_i y_k\,dS_l.
$$

The antisymmetry of the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) kills the last term. Consequently, for the ordinary oriented comoving surface element $d\mathbf S$,

$$
\boxed{\mathbf J=-\frac{a^2\dot D}{4\pi G}
\int_{\Sigma_L}\Phi_i\,\mathbf y\times d\mathbf S.}
$$

The original PDF prints a different coefficient, $-\dot D/(4\pi G\bar\rho_m a^2)$. That coefficient does not follow from its own mass measure and velocity equation and has the wrong dimensions for total [angular momentum](../../../../../angular-momentum.md). The corrected coefficient above also gives the time dependence consistent with the paper's later tensor expression; this is a source typo, not a TeX transcription issue.

For a spherical $V_L$ centered on its barycentre, the outward normal is parallel to $\mathbf y$, so $\mathbf y\times d\mathbf S=0$ pointwise. Hence

$$
\boxed{\mathbf J=0\quad\text{for a spherical initial region}.}
$$

For an [equipotential surface](../../../../../equipotential-surface.md), $\Phi_i=\Phi_*$ on $\Sigma_L$, and

$$
\epsilon_{jkl}\int_{\Sigma_L}y_k\,dS_l
=\epsilon_{jkl}\int_{V_L}\partial_l y_k\,d^3x_i
=\epsilon_{jkl}\delta_{kl}\operatorname{Vol}(V_L)=0.
$$

Therefore

$$
\boxed{\mathbf J=0\quad\text{if the initial boundary is an equipotential}.}
$$

The second conclusion holds for any boundary shape at this order, not just a sphere.

To extract the leading tidal torque, expand the initial [peculiar gravitational potential](../../../../../peculiar-gravitational-potential.md) about the barycentre using its [Taylor series](../../../../../taylor-series.md):

$$
\Phi_i(\hat{\mathbf x}_i+\mathbf y)
=\Phi_0+g_k y_k+\frac12H_{km}y_ky_m+\cdots,
\qquad
H_{km}=\partial_k\partial_m\Phi_i(\hat{\mathbf x}_i).
$$

The constant has no force; $\mathbf g$ has zero integrated torque because the first mass moment vanishes. With the [mass second-moment tensor](../../../../../mass-second-moment-tensor.md)

$$
I_{km}=\rho_0\int_{V_L}y_ky_m\,d^3x_i,
$$

we obtain

$$
J_j=-\frac{a^2\dot D}{4\pi G\rho_0}
\epsilon_{jkl}H_{lm}I_{km}
=\frac{\dot D}{4\pi G\bar\rho_m a}
\epsilon_{jkl}H_{km}I_{ml}.
$$

The second equality swaps the indices $k,l$ and uses the symmetry of both tensors. Define the initial acceleration [tidal tensor](../../../../../tidal-tensor.md) by

$$
T_{km}=-\partial_k\partial_m\Phi_i(\hat{\mathbf x}_i)=-H_{km}.
$$

Then the formula in the question has exactly the stated sign:

$$
\boxed{J_j=-\frac{\dot D}{4\pi G\bar\rho_m a}
\epsilon_{jkl}T_{km}I_{ml}.}
$$

If one defines $T$ as the positive [Hessian matrix](../../../../../hessian-matrix.md) of $\Phi_i$ instead, the displayed contraction has a plus sign. Defining the convention is essential. Also, the paper's $I$ is a [mass second-moment tensor](../../../../../mass-second-moment-tensor.md); the mechanical [inertia tensor](../../../../../inertia-tensor.md) is $\operatorname{tr}(I)\mathbf1-I$.

Only the anisotropic parts contribute: a multiple of the identity produces zero contraction with the [Levi-Civita symbol](../../../../../levi-civita-symbol.md). In axes where $I=\operatorname{diag}(I_1,I_2,I_3)$, for example,

$$
J_1=\frac{\dot D}{4\pi G\bar\rho_m a}T_{23}(I_2-I_3).
$$

Thus a spherical region or tensors sharing principal axes have zero leading torque; unequal principal moments together with off-diagonal tidal components create spin. The [Taylor series](../../../../../taylor-series.md) truncation assumes that higher spatial derivatives of the tidal field are sufficiently small across the region.

In an [Einstein-de Sitter universe](../../../../../einstein-de-sitter-universe.md), $a\propto t^{2/3}$, $D\propto a$, and $\bar\rho_m\propto a^{-3}$. The initial $I$ and $T$ are time independent, so

$$
\boxed{\mathbf J\propto a^2\dot D\propto t^{4/3}t^{-1/3}
\propto t.}
$$

This is early-time growth for fixed initial matter, before collapse invalidates the extrapolation. It does not predict indefinite linear spin growth for a virialized halo.

Two reasons for only approximate agreement with simulations are that nonlinear collapse and [shell crossing](../../../../../shell-crossing.md) change the trajectories and the tidal field, invalidating the first-order displacement and fixed leading [tidal tensor](../../../../../tidal-tensor.md); and that real halos undergo [dark-matter halo mergers](../../../../../dark-matter-halo-merger.md), anisotropic accretion, and exchange of material and [angular momentum](../../../../../angular-momentum.md), so the halo identified at a later time need not be the same isolated collection of initial particles. These processes can change both the magnitude and the direction of the spin.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
