<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Cauchy's stress hypothesis](../../../cauchy-s-stress-hypothesis.md) says that [traction](../../../traction.md) across a cut depends locally on its point, time and oriented normal, rather than on the global shape of the cut. Here all areas and normals are referential: $E$ is a fixed material region in reference coordinates, $\rho_R$ its mass [density](../../../density.md) per reference volume, $v$ the current particle velocity, $b$ [body force](../../../body-force.md) per unit mass, and $s_R$ force per unit reference area. The time derivative on the left is total material momentum rate; the two right terms are contact and [body forces](../../../body-force.md).

A shrinking pillbox gives $s_R(-N)=-s_R(N)$. In a shrinking tetrahedron the volume contributions scale as its linear size cubed, whereas face forces scale as size squared. Their leading balance expresses [traction](../../../traction.md) on an arbitrary face as the normal-component-weighted sum of [tractions](../../../traction.md) on three coordinate faces. Defining those three [tractions](../../../traction.md) as tensor columns gives $\boxed{s_R(N)=T_RN}$. Applying the [divergence theorem](../../../divergence-theorem.md) to [momentum balance](../../../momentum-conservation.md) and localizing over arbitrary $E$ then yields

$$
\boxed{\rho_R\dot v=\operatorname{Div}T_R+\rho_Rb.}
$$

The referential tensor is the [first Piola-Kirchhoff stress](../../../first-piola-kirchhoff-stress-tensor.md) and need not be [symmetric](../../../symmetric-relation.md); it should not be silently identified with the spatial [Cauchy stress](../../../cauchy-stress-tensor.md).

[Incompressibility](../../../incompressible-flow.md) is $\boxed{\det F=1}$. For a [homogeneous hyperelastic material](../../../homogeneous-hyperelastic-material.md) the referential [constitutive relation](../../../constitutive-equation.md) becomes

$$
\boxed{T_R=DW(F)-p\operatorname{cof}F=DW(F)-pF^{-\mathsf T}\quad(\det F=1),}
$$

where the undetermined scalar [pressure](../../../pressure-split.md) $p$ enforces the [constraint](../../../constraint-mechanics.md). Homogeneity removes explicit reference-position dependence from $W$, not the possible spatial variation of that [pressure](../../../pressure-split.md).

For the [neo-Hookean](../../../neo-hookean-solid.md) energy, $DW=2\alpha F$. For the positive diagonal ansatz the nominal principal stresses are $t_i=2\alpha v_i-p/v_i$. Since $F$ is constant, [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) requires $\operatorname{cof}F\nabla p=0$, so $p$ is constant. Stress-free endfaces give $\boxed{p=2\alpha v_3^2>0}$. The side normals include $(0,-1,0)$ and $\pm(\sqrt3/2,1/2,0)$, so their prescribed [tractions](../../../traction.md) force $\boxed{t_1=t_2=T}$.

For fixed positive $p$, the scalar function $2\alpha v-p/v$ is [strictly increasing](../../../strictly-increasing-function.md) on $v>0$. Thus equality of the two nominal stresses implies $v_1=v_2=v$. [Incompressibility](../../../incompressible-flow.md) gives $v_3=v^{-2}$, and substitution gives

$$
\boxed{T=2\alpha(v-v^{-5}),\qquad p=2\alpha v^{-4}.}
$$

The load function has derivative $2\alpha(1+5v^{-6})>0$, tends to minus infinity as $v\downarrow0$ and to infinity as $v\to\infty$. It therefore determines exactly one positive $v$ for every specified load, with $v\geq1$ for outward [tensile](../../../tension.md) $T\geq0$. The resulting constant stress satisfies [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) and every prescribed face [traction](../../../traction.md), proving existence and [uniqueness](../../../uniqueness.md) within the requested positive diagonal class. It does not claim [uniqueness](../../../uniqueness.md) among all possible nonhomogeneous [deformations](../../../deformation-mechanics.md). This is the [equibiaxial dead loading of a neo-Hookean prism](../../../equibiaxial-dead-loading-of-a-neo-hookean-prism.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2008](../../2008-split.md)
3. [Past exam of the solid mechanics course of the University of Oxford](../../split.md)
4. [Solid mechanics course of the University of Oxford](../../../solid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
