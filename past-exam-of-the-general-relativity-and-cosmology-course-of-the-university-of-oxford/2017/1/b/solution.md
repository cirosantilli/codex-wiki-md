<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [metric signature](../../../../metric-signature.md) $(-,+,+,+)$ and a bulk [four-velocity](../../../../four-velocity.md) normalized by $u^\alpha u_\alpha=-c^2$. A [perfect fluid in general relativity](../../../../perfect-fluid-in-general-relativity.md) is isotropic in its local [rest frame](../../../../rest-frame.md), with no rest-frame energy flux or anisotropic stress. In an [orthonormal frame in spacetime](../../../../orthonormal-frame-in-spacetime.md) comoving with that fluid,

$$
u^{\hat\alpha}=(c,0,0,0),\qquad
T^{\hat\alpha\hat\beta}
=\operatorname{diag}(\rho c^2,p,p,p).
$$

Here $\rho$ is rest-frame [energy density](../../../../energy-density.md) divided by $c^2$, including random kinetic energy, and $p$ is isotropic [pressure](../../../../pressure-split.md). For a particle gas, $p=\tfrac13\int\mathbf p\cdot\mathbf v\,dn$ and $\rho c^2=\int E\,dn$, with $dn$ the rest-frame particle distribution. Isotropy makes the off-diagonal spatial stresses and net energy flux vanish.

Introduce the [spatial projector of a timelike congruence](../../../../spatial-projector-of-a-timelike-congruence.md)

$$
P^{\alpha\beta}=g^{\alpha\beta}+\frac{u^\alpha u^\beta}{c^2}.
$$

The only isotropic decomposition with the preceding components is

$$
T^{\alpha\beta}=\rho\,u^\alpha u^\beta+pP^{\alpha\beta}.
$$

Since both sides are [tensors](../../../../tensor.md), equality in the comoving [orthonormal frame in spacetime](../../../../orthonormal-frame-in-spacetime.md) establishes

$$
\boxed{
T^{\alpha\beta}
=\left(\rho+\frac p{c^2}\right)u^\alpha u^\beta
+p\,g^{\alpha\beta}.
}
$$

Coordinate-independent definitions of the two [scalar fields](../../../../scalar-field.md) are

$$
\boxed{
\rho=\frac{T^{\alpha\beta}u_\alpha u_\beta}{c^4},
\qquad
p=\frac13P_{\alpha\beta}T^{\alpha\beta}.
}
$$

Thus $\rho$ is not, in general, only the sum of the particle rest masses per volume.

**The microscopic averaging notation needs a normalization qualification.** The [normalization of an averaged four-velocity](../../../../normalization-of-an-averaged-four-velocity.md) matters because a literal average of normalized microscopic [four-velocities](../../../../four-velocity.md) is not normally a normalized bulk [four-velocity](../../../../four-velocity.md). For example, six equally weighted streams with the same ordinary speed $v$, directed along the positive and negative coordinate axes, have an isotropic velocity distribution and

$$
\langle v^\alpha\rangle=(\gamma c,0,0,0),\qquad
\langle v^\alpha\rangle\langle v_\alpha\rangle=-\gamma^2c^2,
\qquad
\gamma=(1-v^2/c^2)^{-1/2}>1.
$$

The physical rest-frame bulk [four-velocity](../../../../four-velocity.md) is $(c,0,0,0)$, not this unnormalized average. Even taking the source's schematic kinetic expression literally with prefactor $\rho_s$ gives

$$
T^{00}=\rho_s\gamma^2c^2,\qquad
p=\frac{\rho_s\gamma^2v^2}{3}.
$$

Substituting $u=\langle v\rangle$ and the same $\rho_s$ into the claimed fluid expression would instead increase $T^{00}$ by $p(\gamma^2-1)$. The standard result therefore requires a normalized bulk velocity and a carefully defined rest-frame total [energy density](../../../../energy-density.md); it does not follow with both microscopic identifications interpreted literally. More generally the bulk velocity can be defined as the future-directed timelike energy eigenvector of the [stress-energy tensor](../../../../stress-energy-tensor-split.md).

The equation $\nabla_\alpha T^{\alpha\beta}=0$ is local [stress-energy conservation](../../../../stress-energy-conservation.md). In a weak gravitational field and the nonrelativistic limit its leading energy component gives [mass conservation](../../../../mass-conservation.md),

$$
\partial_t\rho+\boldsymbol\nabla\cdot(\rho\mathbf v)=0,
$$

while its spatial components give [momentum conservation](../../../../momentum-conservation.md), or the inviscid [Euler equations](../../../../euler-equations-for-an-inviscid-fluid-split.md)

$$
\rho(\partial_t+\mathbf v\cdot\boldsymbol\nabla)\mathbf v
=-\boldsymbol\nabla p-\rho\boldsymbol\nabla\Phi.
$$

The next energy order gives conservation of internal plus kinetic energy, including pressure work and gravitational work. These are local conservation laws, not an assertion that arbitrary curved [spacetimes](../../../../spacetime.md) possess a global conserved total energy.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
