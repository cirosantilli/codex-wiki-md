<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the adiabatic form of [ideal magnetohydrodynamics](../../../../../ideal-magnetohydrodynamics.md): heat conduction and external heating are absent, so $\rho De/Dt=-p\nabla\cdot\mathbf u$. Infinite electrical conductivity and zero viscosity alone would not remove the thermal source terms on the cover page. If those terms are retained, the energy equation below must acquire $\nabla\cdot(\lambda\nabla T)+\epsilon$ on its right-hand side.

Expanding the [continuity equation](../../../../../continuity-equation.md) gives its conservative form $\partial_t\rho+\nabla\cdot(\rho\mathbf u)=0$. Using it to expand the conservative [momentum](../../../../../momentum.md) derivative gives

$$
\partial_t(\rho\mathbf u)+\nabla\cdot(\rho\mathbf u\mathbf u)
=\rho\frac{D\mathbf u}{Dt}.
$$

For $\nabla\cdot\mathbf B=0$, the [Lorentz force density](../../../../../lorentz-force-density.md) is the divergence of the magnetic [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md):

$$
\mathbf j\times\mathbf B
=\frac1{\mu_0}\left[(\mathbf B\cdot\nabla)\mathbf B-\nabla(B^2/2)\right]
=\nabla\cdot\mathsf T,
\qquad
\mathsf T=\frac1{\mu_0}\left(\mathbf B\mathbf B-\frac12B^2\mathsf I\right).
$$

Combining these identities with [momentum](../../../../../momentum.md) balance proves

$$
\boxed{\partial_t(\rho\mathbf u)+
\nabla\cdot(\rho\mathbf u\mathbf u+p\mathsf I-\mathsf T)
=-\rho\nabla\Phi.}
$$

The dyadic stress contains both [magnetic tension](../../../../../magnetic-tension.md) and [magnetic pressure](../../../../../magnetic-pressure.md); the sign in the flux is fixed by moving the magnetic force to the left.

For the energy equation, first dot [momentum](../../../../../momentum.md) balance with $\mathbf u$ and add the adiabatic internal-energy equation. The [continuity equation](../../../../../continuity-equation.md) converts their [material derivatives](../../../../../material-derivative.md) into conservative derivatives, while $\mathbf u\cdot\nabla p+p\nabla\cdot\mathbf u=\nabla\cdot(p\mathbf u)$. The result is

$$
\partial_t\left(\frac12\rho u^2+\rho e\right)
+\nabla\cdot\left[\mathbf u\left(\frac12\rho u^2+\rho e+p\right)\right]
=-\rho\mathbf u\cdot\nabla\Phi+\mathbf u\cdot(\mathbf j\times\mathbf B).
$$

The [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) gives the magnetic counterpart. In fact,

$$
\begin{aligned}
\partial_t\frac{B^2}{2\mu_0}
&=\frac1{\mu_0}\mathbf B\cdot\nabla\times(\mathbf u\times\mathbf B)\\
&=\frac1{\mu_0}\nabla\cdot[(\mathbf u\times\mathbf B)\times\mathbf B]
-\mathbf u\cdot(\mathbf j\times\mathbf B).
\end{aligned}
$$

Thus the outward [Poynting vector](../../../../../poynting-vector.md) is $(\mathbf B\times\mathbf u)\times\mathbf B/\mu_0$, and magnetic work cancels the fluid work. Finally, the [continuity equation](../../../../../continuity-equation.md) implies

$$
\partial_t(\rho\Phi)+\nabla\cdot(\rho\Phi\mathbf u)
=\rho\partial_t\Phi+\rho\mathbf u\cdot\nabla\Phi.
$$

Adding all three identities gives [ideal magnetohydrodynamic energy conservation](../../../../../ideal-magnetohydrodynamic-energy-conservation.md) in the required local form:

$$
\boxed{\partial_t\mathcal E+\nabla\cdot\mathbf F=\rho\partial_t\Phi,}
$$

where

$$
\begin{aligned}
\mathcal E&=\frac12\rho u^2+\rho e+\rho\Phi+\frac{B^2}{2\mu_0},\\
\mathbf F&=\rho\mathbf u\left(e+\frac p\rho+\frac12u^2+\Phi\right)
+\frac1{\mu_0}(\mathbf B\times\mathbf u)\times\mathbf B.
\end{aligned}
$$

The [magnetic energy](../../../../../magnetic-energy.md) coefficient is $1/(2\mu_0)$, as in the original PDF. For a self-consistent, time-dependent gravitational field this local balance should not be confused with a global self-gravitating energy integral: the latter uses gravitational field energy, or the familiar one-half factor in $\int\rho\Phi$ after the field is eliminated.

Work in the [shock frame](../../../../../shock-frame.md) of a thin planar discontinuity, with normal speed $u>0$. A smooth [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) has no finite jump through a vanishingly thin front; its advected contribution cancels using the common mass flux. Integrating the conservation laws gives constant normal mass, [momentum](../../../../../momentum.md) and energy fluxes, together with the normal-field and tangential-electric-field conditions of the [ideal magnetohydrodynamic shock conditions](../../../../../ideal-magnetohydrodynamic-shock-conditions.md).

For a [parallel magnetohydrodynamic shock](../../../../../parallel-magnetohydrodynamic-shock.md), $\mathbf B=B_n\mathbf n$ and $\mathbf u=u\mathbf n$. The magnetic solenoidal constraint makes $B_n$ the same on both sides. The normal [momentum](../../../../../momentum.md) flux is $\rho u^2+p-B_n^2/(2\mu_0)$; its magnetic term is therefore identical upstream and downstream. The [Poynting vector](../../../../../poynting-vector.md) is zero because $\mathbf u\times\mathbf B=0$. Hence the nontrivial jumps are exactly the [Rankine-Hugoniot conditions for a perfect gas](../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md):

$$
\boxed{\rho_1u_1=\rho_2u_2,
\qquad \rho_1u_1^2+p_1=\rho_2u_2^2+p_2,
\qquad \frac12u_1^2+h_1=\frac12u_2^2+h_2,}
$$

with [specific enthalpy](../../../../../specific-enthalpy.md) $h=\gamma p/[(\gamma-1)\rho]$. Physically, motion along the straight field neither bends it nor compresses its transverse flux. The field consequently provides no changed stress or energy flux in this purely parallel geometry. This conclusion does not apply to a shock that develops a transverse [magnetic field](../../../../../magnetic-field.md).

For a [perpendicular magnetohydrodynamic shock](../../../../../perpendicular-magnetohydrodynamic-shock.md), the [magnetic field](../../../../../magnetic-field.md) is tangential and the [velocity](../../../../../velocity.md) normal. Steady induction makes $uB$ continuous, while the [continuity equation](../../../../../continuity-equation.md) makes $\rho u$ continuous. Dividing gives the [magnetic flux freezing](../../../../../magnetic-flux-freezing.md) relation

$$
\boxed{\frac{B_1}{\rho_1}=\frac{B_2}{\rho_2}.}
$$

Put $x=\rho_2/\rho_1$, so $u_2=u_1/x$ and $B_2=xB_1$. Constant normal [momentum](../../../../../momentum.md) flux now reads $\rho u^2+p+B^2/(2\mu_0)$. Substitution gives

$$
\boxed{p_2=p_1+\rho_1u_1^2\left(1-\frac1x\right)
+\frac{B_1^2}{2\mu_0}(1-x^2).}
$$

The magnetic correction is negative for compression: part of the incoming ram [pressure](../../../../../pressure.md) builds [magnetic pressure](../../../../../magnetic-pressure.md) instead of thermal [pressure](../../../../../pressure.md).

Here the [Poynting vector](../../../../../poynting-vector.md) has normal component $uB^2/\mu_0$. Divide the constant energy flux by the nonzero mass flux to obtain

$$
\frac12u_1^2+\frac{\gamma p_1}{(\gamma-1)\rho_1}
+\frac{B_1^2}{\mu_0\rho_1}
=\frac12u_2^2+\frac{\gamma p_2}{(\gamma-1)\rho_2}
+\frac{B_2^2}{\mu_0\rho_2}.
$$

With $v_{A1}^2=B_1^2/(\mu_0\rho_1)$, this gives the second expression for downstream [pressure](../../../../../pressure.md):

$$
\boxed{p_2=xp_1+\frac{\gamma-1}{\gamma}\rho_1x
\left[\frac12u_1^2\left(1-\frac1{x^2}\right)+v_{A1}^2(1-x)\right].}
$$

In this expression $x$ is the only downstream unknown. Equating the two [pressure](../../../../../pressure.md) expressions and multiplying by $2\gamma x/\rho_1$ yields

$$
(x-1)F(x)=0,
$$

up to an overall minus sign, where $c_1^2=\gamma p_1/\rho_1$ and

$$
\boxed{F(x)=(2-\gamma)v_{A1}^2x^2
+[(\gamma-1)u_1^2+2c_1^2+\gamma v_{A1}^2]x
-(\gamma+1)u_1^2.}
$$

The discarded factor $x=1$ is the unchanged state, not a compressive shock. This derives the polynomial for the [compression ratio of a perpendicular magnetohydrodynamic shock](../../../../../compression-ratio-of-a-perpendicular-magnetohydrodynamic-shock.md) without omitting its trivial branch.

For the usual physical [adiabatic index](../../../../../heat-capacity-ratio.md) $1<\gamma\le2$, $F$ is strictly increasing for positive $x$, has $F(0)<0$, and has one positive root. Since

$$
F(1)=2(c_1^2+v_{A1}^2-u_1^2),
$$

that root is greater than one precisely when $u_1^2>c_1^2+v_{A1}^2$. The necessity is not limited to $\gamma\le2$: for any $\gamma>1$, eliminating $u_1^2$ using $F(x)=0$ gives

$$
\frac{p_2}{\rho_1}
=\frac{c_1^2[(\gamma+1)x-(\gamma-1)]/\gamma
+(\gamma-1)v_{A1}^2(x-1)^3/2}
{D},\qquad D=(\gamma+1)-(\gamma-1)x.
$$

For $x>1$, positive downstream [pressure](../../../../../pressure.md) requires $D>0$ when $c_1^2+v_{A1}^2>0$. Moreover,

$$
u_1^2-c_1^2-v_{A1}^2
=\frac{(x-1)\{(\gamma+1)c_1^2+v_{A1}^2[(2-\gamma)x+\gamma+1]\}}{D}>0.
$$

The bracket is positive throughout $1<x<(\gamma+1)/(\gamma-1)$, even when $\gamma>2$. The exactly cold unmagnetized limit gives the familiar strong-shock upper compression ratio directly. Thus the physical compressive branch requires

$$
\boxed{u_1^2>c_1^2+v_{A1}^2.}
$$

The PDF's final $v_1$ denotes this same incoming speed $u_1$. The right side is the squared speed of a perpendicular fast [magnetosonic wave](../../../../../magnetosonic-wave.md): the upstream flow must be super-fast-magnetosonic so that this compressive signal cannot run upstream against the incoming flow. At equality the shock amplitude vanishes into a characteristic disturbance.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
