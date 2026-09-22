<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For an axisymmetric [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md), the vacuum [Laplace equation in cylindrical coordinates](../../../../../laplace-equation-in-cylindrical-coordinates.md) is $R^{-1}\partial_R(R\partial_R\Phi)+\partial_z^2\Phi=0$. Use [separation of variables](../../../../../separation-of-variables.md), $\Phi=X(R)Z(z)$. Dividing by $XZ$ and setting the separated constant to $k^2$, with $k>0$, gives

$$
Z''=k^2Z,\qquad X''+\frac1RX'+k^2X=0.
$$

The first equation has solutions $e^{\pm kz}$; with $u=kR$, the second is the order-zero [Bessel differential equation](../../../../../bessel-differential-equation.md). Regularity at the axis selects the [Bessel function of the first kind](../../../../../bessel-function-of-the-first-kind.md) $J_0(kR)$, rather than the singular [Bessel function of the second kind](../../../../../bessel-function-of-the-second-kind.md) $Y_0$. Thus

$$
\boxed{\Phi_k(R,z)=e^{\pm kz}J_0(kR).}
$$

There are also zero-separation-constant modes, and other boundary conditions can select other separated families. For a localized reflection-symmetric [thin disk](../../../../../thin-disk.md), decay away from the disk selects $e^{-k|z|}$ on the respective half-spaces.

Apply the [divergence theorem](../../../../../divergence-theorem.md) to the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) across a narrow pillbox enclosing disk area. Writing the volume [mass density](../../../../../density.md) as $\Sigma(R)\delta(z)$ gives

$$
\Phi_z(R,0^+)-\Phi_z(R,0^-)=4\pi G\Sigma(R).
$$

Reflection symmetry makes $\Phi_z(R,0^+)=2\pi G\Sigma(R)$. A superposition of the regular vacuum modes therefore satisfies

$$
\Phi=\int_0^\infty S(k)J_0(kR)e^{-k|z|}\,dk,\qquad -\int_0^\infty kS(k)J_0(kR)\,dk=2\pi G\Sigma(R).
$$

The order-zero [Hankel transform](../../../../../hankel-transform.md) and its inversion now determine the [Hankel representation of thin-disk gravity](../../../../../hankel-representation-of-thin-disk-gravity.md):

$$
\boxed{S(k)=-2\pi G\int_0^\infty\Sigma(R)J_0(kR)R\,dR.}
$$

The sign is fixed by the positive derivative of an attractive [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) above the disk. For ordinary finite disks the representation uses the isolated boundary condition, fixing any extra vacuum field or additive constant. Infinite scale-free disks require suitable regularization of the potential itself.

Equatorial [circular orbit](../../../../../circular-orbit.md) balance is $v_c^2=R\Phi_R(R,0)$. Using $J_0'(u)=-J_1(u)$ in the [Hankel representation of thin-disk gravity](../../../../../hankel-representation-of-thin-disk-gravity.md) gives

$$
\boxed{v_c^2(R)=-R\int_0^\infty kS(k)J_1(kR)\,dk.}
$$

Differentiation under the integral is justified by convergence for regular models, or by first working off the disk and taking the limiting radial field.

Write $C=\Sigma_0R_0$. For the [Mestel disk](../../../../../mestel-disk.md), the supplied [Bessel function](../../../../../bessel-function.md) integral gives $S(k)=-2\pi GC/k$ for $k>0$. The [circular speed](../../../../../circular-speed.md) is then

$$
v_c^2=2\pi GC R\int_0^\infty J_1(kR)\,dk=2\pi GC.
$$

Meanwhile the interior [mass](../../../../../mass.md) is $M(R)=2\pi\int_0^R(C/s)s\,ds=2\pi CR$. Consequently

$$
\boxed{v_c^2=2\pi G\Sigma_0R_0=\frac{GM(R)}R.}
$$

The [Mestel disk](../../../../../mestel-disk.md) has a [flat galaxy rotation curve](../../../../../flat-galaxy-rotation-curve.md), despite its nonspherical geometry.

Its infinite total [mass](../../../../../mass.md) prevents setting the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) to zero at infinity. Indeed the integral for $\Phi$ diverges at $k=0$ because $S(k)\sim1/k$. Subtracting the potential at a reference point removes this additive divergence. As an explicit check, the [Mestel disk potential-density pair](../../../../../mestel-disk-potential-density-pair.md) is

$$
\Phi=2\pi GC\log\!\left(\frac{\sqrt{R^2+z^2}+|z|}{R_*}\right).
$$

It is harmonic for $z\ne0$, its vertical derivative jump is $4\pi GC/R$, and $R\Phi_R(R,0)=2\pi GC$. Equivalently, an [Abel regularization of an oscillatory integral](../../../../../abel-regularization-of-an-oscillatory-integral.md) with damping factor $e^{-ak}$ in the radial-field integral gives $R\int_0^\infty e^{-ak}J_1(kR)dk=1-a/\sqrt{a^2+R^2}$, which tends to one as $a\downarrow0$. The force is well-defined although the unreferenced potential is not.

**The equality with $GM(R)/R$ is special to the Mestel disk, not a thin-disk shell theorem.** The [spherical shell theorem](../../../../../spherical-shell-theorem.md) normally makes that formula possible, but does not apply to an [astrophysical disk](../../../../../astrophysical-disk.md). Exterior annuli exert outward radial [gravitational acceleration](../../../../../gravitational-acceleration.md) inside their radii, while interior annuli do not act exactly as point masses at the origin. For this particular scale-free [surface density](../../../../../surface-density-of-a-disk.md), their combined contributions happen to produce the same result as the interior [mass](../../../../../mass.md) expression. Changing the radial [surface density](../../../../../surface-density-of-a-disk.md) or truncating the disk generally destroys the equality: [enclosed mass does not determine a disc rotation curve](../../../../../enclosed-mass-does-not-determine-a-disc-rotation-curve.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
