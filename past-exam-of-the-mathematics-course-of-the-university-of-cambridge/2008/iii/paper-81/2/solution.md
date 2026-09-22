<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A precise [stratification–rotation analogy](../../../../../stratification-rotation-analogy.md) uses constant $N$, ideal fluid, and independence of one horizontal coordinate. For the stratified system take $\partial_y=0$, $v=0$, and allow prescribed forces $(F_x,0,F_z)$. The possibly nonlinear [Boussinesq equations](../../../../../boussinesq-equations.md) are

$$
Du=-p_x+F_x,\qquad Dw=-p_z+\sigma+F_z,
\qquad D\sigma=-N^2w,\qquad u_x+w_z=0,
\qquad D=\partial_t+u\partial_x+w\partial_z.
$$

For the unstratified system choose right-handed coordinates $(X,Y,Z)=(z,y,-x)$, rotation $2\boldsymbol\Omega=N\mathbf e_Z$, and $\partial_Y=0$. Its rotating Euler equations, with the static gravitational and centrifugal contributions absorbed into the background pressure, are

$$
D_RU-NV=-P_X+\mathcal F_X,\qquad
D_RV+NU=\mathcal F_Y,\qquad
D_RW=-P_Z+\mathcal F_Z,\qquad U_X+W_Z=0,
$$

where $D_R=\partial_t+U\partial_X+W\partial_Z$. The identification is

$$
\boxed{U=w,\quad V=\sigma/N,\quad W=-u,\quad P=p,
\quad (\mathcal F_X,\mathcal F_Y,\mathcal F_Z)=(F_z,0,-F_x).}
$$

Then $D_R=D$, $P_X=p_z$, and $P_Z=-p_x$, proving the component-by-component equivalence. In particular, [buoyancy perturbation](../../../../../buoyancy-perturbation.md) maps to transverse rotating velocity, and stratified horizontal velocity maps to rotation-axis velocity. The mapping permits arbitrary prescribed forces in the two-dimensional plane, but no transverse force: a transverse force in the rotating problem would create a source in the stratified buoyancy equation. A transverse stratified force would also invalidate $v=0$. Constant $N$ is essential to this constant-rotation equivalence.

A physical [free surface](../../../../../free-surface.md) introduces extra structure beyond the interior equations. After subtracting [hydrostatic pressure](../../../../../hydrostatic-pressure.md), its zero total pressure condition gives $p=g\eta$ to first order, together with the kinematic condition $\eta_t=w$ for the stratified vertical displacement. The mapping takes this normal velocity into $U$, whereas an actual rotating free surface normal to its physical vertical $Z$ has normal velocity $W$ and a displacement along $Z$. The image of the stratified horizontal surface is a vertical surface in the rotating coordinates. Consequently **the physical free-surface problems are not analogous**, although deliberately mapped rigid boundaries or mathematical boundary data can be.

For the first prescribed force, the steady linear stratified equations are satisfied by

$$
\mathbf u=(u(z),0,0),\qquad
p=f(x)e^{imz}+b(z),\qquad
\sigma=imf(x)e^{imz}+b'(z).
$$

Real parts are understood. The horizontal pressure gradient balances the force; the vertical pressure gradient is balanced by [buoyancy](../../../../../buoyancy.md); and $w=0$ satisfies buoyancy conservation and [incompressible flow](../../../../../incompressible-flow.md). Thus neither $u(z)$ nor $b(z)$ is fixed by the steady equations alone.

Initial rest and switching on in the unbounded fluid remove this ambiguity by [causal pressure adjustment by internal waves](../../../../../causal-pressure-adjustment-by-internal-waves.md). Work with the $e^{imz}$ coefficient and let $\widehat F(q)$ be the horizontal [Fourier transform](../../../../../fourier-transform.md) of $f'(x)$. For an abrupt switch at time zero, elimination in the linear equations gives

$$
\Omega(q)=\frac{Nq}{\sqrt{q^2+m^2}},\qquad
\widehat u(q,t)=\frac{m^2\widehat F(q)}{(q^2+m^2)\Omega(q)}\sin(\Omega(q)t),
$$



$$
\widehat p(q,t)=-\frac{i\widehat F(q)}q
\left[1-\frac{m^2}{q^2+m^2}\cos(\Omega(q)t)\right].
$$

At $q=0$ the bracket cancels the apparent singularity at every finite time. The persistent pressure term is the symmetric antiderivative of the force: the inverse transform of $-i\widehat F/q$, interpreted as a [Cauchy principal value](../../../../../cauchy-principal-value.md), is $f(x)-\varepsilon/2$. The oscillatory part propagates away. To see why its zero-frequency part does not leave an arbitrary offset, note that $\Omega(q)\sim cq$ with $c=N/m$; its long-wave contribution consists of oppositely moving fronts. At fixed $x$, the two far-field values of $f-\varepsilon/2$ are $-\varepsilon/2$ and $+\varepsilon/2$, whose average is zero. Nonzero horizontal [wavenumbers](../../../../../wavenumber.md) give dispersive transients that decay locally. Smooth finite-duration switching changes the transient, not this selected steady limit. Therefore

$$
\boxed{p_\infty=[f(x)-\varepsilon/2]e^{imz},\qquad
b(z)=-\frac{\varepsilon}{2}e^{imz}.}
$$

A spatially constant pressure gauge is immaterial. The long-wave [group velocity](../../../../../group-velocity.md) $c=N/m$ gives the adjustment scale: the elapsed time since switching must satisfy $Nt\gg1$ and $(N/m)t\gg |x|+x_1$, and exceed the switching duration. These are asymptotic conditions, **not an assertion of exact equilibration after a finite time**; the full [dispersion relation](../../../../../dispersion-relation.md) allows tails. The same long-wave limit gives $u_\infty=\varepsilon m e^{imz}/(2N)$ if desired. Equal-amplitude outward fronts leave opposite pressure offsets and the same velocity on their two sides.

For the force depending instead on $y$, any steady linear horizontal momentum balance requires $p_x=f'(x)e^{i\ell y}$ and $p_y=0$. Their mixed derivatives disagree wherever $f'\ne0$, since $\partial_y p_x=i\ell f'(x)e^{i\ell y}$ but $\partial_xp_y=0$. Hence **no steady linear velocity field can satisfy the equations**, irrespective of whether it is $x$-independent. This statement concerns the linearized problem; nonlinear inertial balances were excluded by the assumptions.

For an unsteady solution put $\mathbf u=(-t\phi_y,t\phi_x,0)$ and take $\sigma=0$. Its horizontal [divergence](../../../../../divergence.md) is zero. The pressure derivatives needed in momentum balance are

$$
p_x=f'(x)e^{i\ell y}+\phi_y,\qquad p_y=-\phi_x,\qquad p_z=0.
$$

Their compatibility is exactly

$$
\boxed{\phi_{xx}+\phi_{yy}=-i\ell f'(x)e^{i\ell y}.}
$$

Thus the [Poisson equation](../../../../../poisson-equation.md) supplies an actual pressure and the proposed velocity solves both momentum equations; the vertical momentum and buoyancy equations hold because $w=\sigma=0$. This flow grows linearly in time, so it remains a valid small-disturbance prediction only while its velocities are small.

As $x_1\to0$ with total force $\varepsilon$ fixed, $f'\to\varepsilon\delta(x)$. Set $\phi=\Phi(x)e^{i\ell y}$. Away from the source $\Phi''-\ell^2\Phi=0$, and decay at both ends requires $\Phi=Ae^{-\ell|x|}$. Integrating across the source gives the jump $\Phi'(0^+)-\Phi'(0^-)=-i\ell\varepsilon$. Since this jump is $-2\ell A$, $A=i\varepsilon/2$, so

$$
\boxed{\phi=\frac{i\varepsilon}{2}e^{i\ell y}e^{-\ell|x|}.}
$$

This verifies the distributional source as well as the decay condition.

The corresponding rotating problem is not expected to reproduce this evanescent accelerating flow. Its forcing varies in $Y$, precisely the coordinate whose independence was required in the [stratification–rotation analogy](../../../../../stratification-rotation-analogy.md). Moreover, $x$ maps to the rotation-axis coordinate $-Z$. At small [Rossby number](../../../../../rossby-number.md), the [Taylor–Proudman theorem](../../../../../taylor-proudman-theorem.md) gives $\partial_Z\mathbf u_R=0$ in the unforced exterior regions. Such nonzero columns cannot decay with $|Z|$, hence cannot reproduce an $e^{-\ell|x|}$ tail. There is also a direct unsteady obstruction to copying the proposed flow: in a homogeneous fluid rotating about the mapped $x$ axis, a mode with nonzero axial [wavenumber](../../../../../wavenumber.md) has [inertial wave](../../../../../inertial-wave.md) frequency of magnitude $N|q|/\sqrt{q^2+\ell^2}$, rather than the zero-frequency horizontal vortical response of the stratified problem. The steady or slowly varying exterior rotating response must be columnar or accompanied by outgoing [inertial waves](../../../../../inertial-wave.md); **the decaying stratified solution is outside the partial analogy**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
