<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the basic [axisymmetric flow](../../../../../axisymmetric-flow.md), $\mathbf u_0=\Omega R\mathbf e_\phi$. The steady radial [Euler equation for fluid motion](../../../../../euler-equations-for-an-inviscid-fluid.md) gives $-\Omega^2R=-p_{0,R}/\rho$; the other components give $p_{0,z}=p_{0,\phi}=0$. Thus, in the absence of an additional body force,

$$
\boxed{p_0(R,z)=p_c+\frac12\rho\Omega^2R^2.}
$$

The additive constant is undetermined without an imposed reference [pressure](../../../../../pressure.md); the rigid boundary does not prescribe a uniform boundary [pressure](../../../../../pressure.md). Its shape is fixed by the container rather than by a free-surface [pressure](../../../../../pressure.md) condition.

Let $v_R,v_\phi,v_z$ be the small [velocity](../../../../../velocity.md) amplitudes and $W=p_1/\rho$ the [pressure](../../../../../pressure.md) amplitude. Linearizing the cylindrical [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) about uniform rotation, the material [derivative](../../../../../derivative.md) is $\partial_t+\Omega\partial_\phi$. The intrinsic [frequency](../../../../../frequency.md) for the stated phase convention is therefore

$$
s=\bar\sigma=\sigma+m\Omega.
$$

The radial and azimuthal curvature terms supply the [Coriolis acceleration](../../../../../coriolis-acceleration.md) terms, giving

$$
isv_R-2\Omega v_\phi=-W_R,\qquad
isv_\phi+2\Omega v_R=-\frac{im}{R}W,\qquad
isv_z=-W_z.
$$

For $s\ne0,\pm2\Omega$, solving these equations gives

$$
v_R=\frac{i(sW_R+2m\Omega W/R)}{s^2-4\Omega^2},\qquad
v_\phi=-\frac{2\Omega W_R+smW/R}{s^2-4\Omega^2},\qquad
v_z=\frac{iW_z}s.
$$

The [incompressible flow](../../../../../incompressible-flow.md) constraint is

$$
\frac1R(Rv_R)_R+\frac{im}{R}v_\phi+(v_z)_z=0.
$$

On substitution, the terms proportional to $m\Omega W_R$ cancel. The remaining equation is

$$
\frac{is}{s^2-4\Omega^2}
\left[\frac1R(RW_R)_R-\frac{m^2W}{R^2}\right]
+\frac is W_{zz}=0,
$$

which proves

$$
\boxed{\frac1R\frac{\partial}{\partial R}(R W_R)-\frac{m^2W}{R^2}
+\left(1-\frac{4\Omega^2}{\bar\sigma^2}\right)W_{zz}=0.}
$$

This is the [pressure](../../../../../pressure.md) equation for [inertial modes in a rigid rotating sphere](../../../../../inertial-modes-in-a-rigid-rotating-sphere.md). The exceptional [frequencies](../../../../../frequency.md) used in the divisions must instead be treated in the original momentum system; they are not needed for the mode below.

A fixed rigid sphere is impermeable, so its normal [velocity](../../../../../velocity.md) vanishes:

$$
R v_R+zv_z=0\qquad(R^2+z^2=r_0^2).
$$

Using the solved amplitudes and multiplying by $s(s^2-4\Omega^2)/i$ gives

$$
\boxed{\bar\sigma^2 R W_R+2m\Omega\bar\sigma W
+(\bar\sigma^2-4\Omega^2)zW_z=0\quad\text{on }r=r_0.}
$$

Equivalently divide by $\bar\sigma^2$ for $\bar\sigma\ne0$. Smoothness means tangential slip is allowed: there is no no-slip condition on these inviscid [normal modes](../../../../../normal-mode.md). Nor is there a condition $W=0$, since the wall supplies the required varying normal [pressure](../../../../../pressure.md).

For an axisymmetric oscillation, $m=0$ and $s=\sigma$. Write $\beta=1-4\Omega^2/\sigma^2$. For $W=z(AR^2+Bz^2+C)$ the radial and vertical operators are

$$
\frac1R(RW_R)_R=4Az,\qquad W_{zz}=6Bz.
$$

The interior [pressure](../../../../../pressure.md) equation therefore requires

$$
2A+3\beta B=0.
$$

The boundary equation becomes

$$
z\left[(2+\beta)AR^2+3\beta Bz^2+\beta C\right]=0.
$$

Substituting $R^2=r_0^2-z^2$, this [polynomial](../../../../../polynomial-split.md) must vanish for every boundary height. Its constant and $z^2$ coefficients consequently give

$$
(2+\beta)Ar_0^2+\beta C=0,\qquad
3\beta B-(2+\beta)A=0.
$$

Together with the interior relation the latter condition is $(4+\beta)A=0$. A nontrivial nonsingular oscillatory solution needs $A\ne0$: if $A=0$ and $\beta\ne0$, the other equations force $B=C=0$. Hence $\beta=-4$, giving

$$
\boxed{\sigma^2=\frac{4\Omega^2}{5},\qquad
B=\frac A6,\qquad C=-\frac{Ar_0^2}{2}.}
$$

The [cubic axisymmetric inertial mode of a rigid sphere](../../../../../cubic-axisymmetric-inertial-mode-of-a-rigid-sphere.md) is explicitly

$$
\boxed{W=A z\left(R^2+\frac{z^2}{6}-\frac{r_0^2}{2}\right),\qquad
\sigma=\pm\frac{2|\Omega|}{\sqrt5}.}
$$

Its cubic [pressure](../../../../../pressure.md) is regular at the axis and centre, and its reconstructed [velocity](../../../../../velocity.md) is divergence free and tangent to the sphere by the preceding identities. The [frequency](../../../../../frequency.md) lies within the [inertial wave](../../../../../inertial-wave.md) band $|\sigma|<2|\Omega|$: [Coriolis acceleration](../../../../../coriolis-acceleration.md), rather than compression or a moving surface, supplies the restoring dynamics. The amplitude $A$ is arbitrary in this linear problem.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
