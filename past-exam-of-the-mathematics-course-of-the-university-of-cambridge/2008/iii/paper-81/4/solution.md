<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The geostrophic [material derivative](../../../../../material-derivative.md) is

$$
\frac{D_g}{Dt}=\partial_t+J(\psi,\cdot)
=\partial_t-\psi_y\partial_x+\psi_x\partial_y.
$$

It advects horizontally with the [geostrophic flow](../../../../../geostrophic-flow.md). The exact [material derivative](../../../../../material-derivative.md) additionally includes horizontal [ageostrophic flow](../../../../../ageostrophic-flow.md) and vertical advection $w\partial_z$. The leading balances are [geostrophic balance](../../../../../geostrophic-balance.md) and the [hydrostatic approximation](../../../../../hydrostatic-approximation.md):

$$
-f_0v=-p_x,\qquad f_0u=-p_y,\qquad 0=-p_z+\sigma.
$$

The conventional [quasi-geostrophic streamfunction](../../../../../quasi-geostrophic-streamfunction.md) is $p=f_0\psi$, after fixing the horizontally uniform reference pressure consistently with the basic buoyancy profile. Therefore

$$
\boxed{\sigma=f_0\psi_z.}
$$

Here and below pressure is divided by reference density, and $\sigma$ is the anomaly about the prescribed background [buoyancy](../../../../../buoyancy.md).

For the zonal average assume periodicity or vanishing boundary terms, so that averages of $x$ derivatives vanish and averaging commutes with $y,z$ derivatives. Put $S(z)=f_0^2/N^2(z)$. Since $\overline{\psi'_x}=0$, the disturbance [quasi-geostrophic potential vorticity](../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md) is $Q'=\psi'_{xx}+\psi'_{yy}+\partial_z(S\psi'_z)$. The zonal part of $\overline{\psi'_xQ'}$ vanishes as $\tfrac12\overline{\partial_x(\psi'_x)^2}$. For the other parts, integration by parts gives

$$
\overline{\psi'_x\psi'_{yy}}
=\partial_y\overline{\psi'_x\psi'_y}
-\tfrac12\overline{\partial_x(\psi'_y)^2}
=\partial_y\overline{\psi'_x\psi'_y},
$$



$$
\overline{\psi'_x\partial_z(S\psi'_z)}
=\partial_z(S\overline{\psi'_x\psi'_z})
-\tfrac12 S\overline{\partial_x(\psi'_z)^2}
=\partial_z(S\overline{\psi'_x\psi'_z}).
$$

As $u'=-\psi'_y$, $v'=\psi'_x$, and $\sigma'=f_0\psi'_z$, the [Eliassen–Palm flux](../../../../../eliassen-palm-flux.md) is

$$
F=\overline{\psi'_x\psi'_y}=-\overline{u'v'},
\qquad G=S\overline{\psi'_x\psi'_z}=\frac{f_0}{N^2}\overline{v'\sigma'}.
$$

We have therefore proved the exact [Taylor identity for quasi-geostrophic flux](../../../../../taylor-identity-for-quasi-geostrophic-flux.md),

$$
\boxed{F_y+G_z=\overline{v'Q'},}
$$

without imposing small amplitude. This identity is algebraic within the [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md); it does not assert validity of that approximation for arbitrary physical flows.

Now linearize about a steady zonal basic flow $\bar u=U(y,z)$, with $\bar Q_y\ne0$ and no mean meridional velocity. The linear [quasi-geostrophic potential-vorticity equation](../../../../../quasi-geostrophic-potential-vorticity-equation.md) is $Q'_t+UQ'_x+v'\bar Q_y=0$. Multiply by $Q'/\bar Q_y$ and average. The advection term is a zonal derivative and vanishes, giving

$$
\mathcal A=\frac{\overline{Q'^2}}{2\bar Q_y},\qquad
\mathcal A_t=-\overline{v'Q'},\qquad
\boxed{\mathcal A_t+F_y+G_z=0.}
$$

This is [quasi-geostrophic wave-activity conservation law](../../../../../quasi-geostrophic-wave-activity-conservation-law.md). The basic-state denominator is time-independent at the retained order; its change caused by the waves is higher order. The [wave activity](../../../../../wave-activity.md) is signed if $\bar Q_y<0$, and the formula cannot be used where that gradient vanishes. The original PDF includes the zonal average over the squared disturbance in this definition.

For the resonant solution it is helpful to avoid squaring an imaginary coefficient as though it were real. Write

$$
U=\beta/\kappa^2,\qquad S=f_0^2/N^2,\qquad
B=iB_0,\quad B_0=\frac{2kf_0U^2}{\beta},\qquad
C=\frac{N^2}{f_0m},\quad m=\pi/H,
$$

where $B_0$ is real. Assume $f_0\ne0$, $\beta\ne0$, and $k\ne0$. Define $c(z)=\cos(mz)$ and $r(z)=(z-H)\sin(mz)$. The complex coefficient of the physical [streamfunction](../../../../../stream-function.md) disturbance is

$$
\psi'=\operatorname{Re}\{\varepsilon e^{ikx}\sin(\ell y)h(z,t)\},
\qquad h=iB_0tc+Cr.
$$

The original PDF contains $Bt\cos(mz)$: the converted TeX's missing $t$ would incorrectly remove the [resonance](../../../../../resonance.md) and fails the differential equations.

For the vertical [potential-vorticity inversion](../../../../../potential-vorticity-inversion.md) operator, $c''=-m^2c$ and $r''=-m^2r+2mc$. Consequently

$$
Q'=\operatorname{Re}\{\varepsilon e^{ikx}\sin(\ell y)q(z,t)\},
\qquad q=-\kappa^2h+2SmCc=-\kappa^2h+2f_0c.
$$

Substitution in the linear [potential-vorticity equation](../../../../../potential-vorticity-evolution-equation.md) gives

$$
q_t+ikUq+ik\beta h
=(-i\kappa^2B_0+2ikUf_0)c=0,
$$

since $\kappa^2B_0=2kf_0U$. Thus this is a genuine [resonant topographic quasi-geostrophic wave](../../../../../resonant-topographic-quasi-geostrophic-wave.md), with linear amplitude growth rather than an assumed stationary wave.

At the flat upper boundary $h_z(H,t)=0$, so $w'(H)=0$. At the lower boundary, linearization of the impermeability condition gives $w'(0)=U\partial_x h_b$, where $h_b=\operatorname{Re}\{\varepsilon H e^{ikx}\sin(\ell y)\}$ is the bottom corrugation. Here $h_z(0,t)=-CHm$ is time-independent, so the specified vertical velocity gives

$$
w'(0)=-\frac{f_0}{N^2}\operatorname{Re}\{\varepsilon e^{ikx}\sin(\ell y)
(\partial_t+ikU)(-CHm)\}
=\operatorname{Re}\{ikU\varepsilon H e^{ikx}\sin(\ell y)\},
$$

using $f_0Cm/N^2=1$. Both boundary conditions are verified. The linear solution is valid while its growing displacement and velocity remain small; it is not a large-time nonlinear solution.

To evaluate all fluxes, use $\overline{\operatorname{Re}(ae^{ikx})\operatorname{Re}(be^{ikx})}=\tfrac12\operatorname{Re}(ab^*)$. The coefficients of $u',v',\sigma'$ are respectively $-\varepsilon\ell\cos(\ell y)h$, $i\varepsilon k\sin(\ell y)h$, and $\varepsilon f_0\sin(\ell y)h_z$. Hence

$$
\overline{u'v'}=0,\qquad \boxed{F=0.}
$$

The products of the $B_0t$ terms alone and the $C$ terms alone are imaginary in the vertical flux and contribute nothing. Only the cross terms remain. Since

$$
c r'-r c'=\sin(mz)\cos(mz)+m(z-H)=:R(z),
$$

we obtain

$$
\overline{v'\sigma'}=-\frac{\varepsilon^2 f_0kB_0Ct}{2}\sin^2(\ell y)R(z),
\qquad
\boxed{G=-\frac{\varepsilon^2 SkB_0Ct}{2}\sin^2(\ell y)R(z).}
$$

Differentiating $R$ gives $R'=m(1+\cos(2mz))=2m\cos^2(mz)$. As $SmC=f_0$,

$$
\boxed{F_y+G_z=-\varepsilon^2 kf_0B_0t\sin^2(\ell y)\cos^2(mz).}
$$

For an independent evaluation of the right side of the [Taylor identity for quasi-geostrophic flux](../../../../../taylor-identity-for-quasi-geostrophic-flux.md), write $q=(2f_0c-\kappa^2Cr)-i\kappa^2B_0tc$. Multiplication of $ikh$ by $q^*$ gives real part $-2kf_0B_0tc^2$, because the remaining real cross terms cancel. Therefore

$$
\boxed{\overline{v'Q'}=-\varepsilon^2 kf_0B_0t\sin^2(\ell y)\cos^2(mz),}
$$

which verifies the flux identity pointwise in $y,z$.

The basic [potential-vorticity gradient](../../../../../potential-vorticity-gradient.md) is $\bar Q_y=\beta$, so the [wave activity](../../../../../wave-activity.md) and its derivative are

$$
\mathcal A=\frac{\varepsilon^2\sin^2(\ell y)}{4\beta}
\left[(2f_0c-\kappa^2Cr)^2+\kappa^4B_0^2t^2c^2\right],
$$



$$
\boxed{\mathcal A_t=\frac{\varepsilon^2\kappa^4B_0^2t}{2\beta}
\sin^2(\ell y)c^2
=\varepsilon^2 kf_0B_0t\sin^2(\ell y)c^2.}
$$

Here $\kappa^4B_0^2/(2\beta)=kf_0B_0$ follows from $U=\beta/\kappa^2$. Thus $\mathcal A_t+F_y+G_z=0$. The growth term involves $B_0^2=|B|^2=-B^2$; the distinction matters because the printed complex coefficient $B$ is imaginary. These formulas evaluate both flux components, their divergence, the buoyancy and PV covariances, and [wave activity](../../../../../wave-activity.md). In particular $G(H)=0$ and $G(0)=\varepsilon^2kf_0B_0Ht\sin^2(\ell y)/2$, so for $\beta>0$ the growing activity is supplied by the positive flux from the lower boundary.

Finally put $W=\pi/\ell$ and write the height-independent mean velocity change as $\delta U(y)$. Since $\delta\bar\psi_y=-\delta U$ and $\delta\bar\psi$ can be chosen independent of height, the mean [potential vorticity](../../../../../potential-vorticity.md) becomes

$$
\bar Q_{\rm final}=f_0+\beta y-\delta U_y.
$$

To be uniform in $y$ this requires $\delta U_y=\beta y-K$ for some constant $K$. Integrating and applying both endpoint conditions gives $\delta U(0)=0$, $\delta U(W)=0$, and hence $K=\beta W/2$. Therefore

$$
\boxed{\delta U(y)=\frac\beta2y(y-W),\qquad
\bar Q_{\rm final}=f_0+\frac{\beta W}{2}.}
$$

The constant is the initial channel-mean [potential vorticity](../../../../../potential-vorticity.md), as also follows from $\int_0^W\delta Q\,dy=-[\delta U]_0^W=0$. This is the [momentum loss from uniform potential-vorticity mixing](../../../../../momentum-loss-from-uniform-potential-vorticity-mixing.md). Averaging the velocity change across the channel gives the momentum change per unit mass,

$$
\boxed{\frac1W\int_0^W\delta U\,dy
=\frac\beta{2W}\left(\frac{W^3}{3}-\frac{W^3}{2}\right)
=-\frac{\beta}{12}\left(\frac\pi\ell\right)^2.}
$$

For positive $\beta$ the mean current is reduced everywhere in the interior. The imposed bottom can exchange momentum with the fluid, so this change is consistent with the complete [conservation of momentum](../../../../../momentum-conservation.md) budget.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
