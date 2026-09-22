<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

**Changing basis and acceleration.** Attach orthonormal [unit vectors](../../../../../unit-vector.md) $\mathbf e_i(t)$ to the rotating frame, with a common origin fixed in the [inertial frame](../../../../../inertial-frame.md). An infinitesimal [rotation](../../../../../rotation-mathematics.md) $d\boldsymbol\theta=\boldsymbol\omega\,dt$ changes a vector fixed in those axes by $d\mathbf A=d\boldsymbol\theta\times\mathbf A$: its tip moves tangentially to the circle about the [rotation](../../../../../rotation-mathematics.md) axis. More generally, write $\mathbf A=\sum_iA_i\mathbf e_i$. Differentiating the components and the rotating basis separately proves the [rotating-frame derivative formula](../../../../../rotating-frame-derivative-formula.md),

$$
\boxed{\left.\frac{d\mathbf A}{dt}\right|_0
=\left.\frac{d\mathbf A}{dt}\right|_S
+\boldsymbol\omega\times\mathbf A.}
$$

<a id="section-c/c10/image-original-geometric-construction-of-the-tangential-change-of-a-vector-during-a-small-positive-rotation-the-change-is-dtheta-crossed-with-a"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-1-c10-rotating-vector.png)

**[Figure 3](#section-c/c10/image-original-geometric-construction-of-the-tangential-change-of-a-vector-during-a-small-positive-rotation-the-change-is-dtheta-crossed-with-a). Original geometric construction of the tangential change of a vector during a small positive rotation; the change is dtheta crossed with A**.

Apply the formula first to position: $\dot{\mathbf r}_0=\mathbf v+\boldsymbol\omega\times\mathbf r$, where $\mathbf v=(d\mathbf r/dt)_S$. Apply it again to both terms. For constant $\boldsymbol\omega$,

$$
\boxed{\ddot{\mathbf r}_0=\mathbf a
+2\boldsymbol\omega\times\mathbf v
+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf r).}
$$

One cross term comes from differentiating $\mathbf v$ in the inertial frame and another from differentiating $\mathbf r$ in $\boldsymbol\omega\times\mathbf r$. The displayed source formula implicitly requires constant [angular velocity](../../../../../angular-velocity.md) and an unaccelerated common origin. For changing [rotation](../../../../../rotation-mathematics.md) rate there is also $\dot{\boldsymbol\omega}\times\mathbf r$; an accelerating origin supplies its own translational [acceleration](../../../../../acceleration.md). Moving the [rotation](../../../../../rotation-mathematics.md) terms to the [force](../../../../../force-split.md) side gives the apparent [Coriolis force](../../../../../coriolis-force.md) and [centrifugal force](../../../../../centrifugal-force.md) with negative signs.

**Southward motion on Earth.** Use local east, north and up axes, with latitude $\lambda$ positive northward. Then $\boldsymbol\Omega=\Omega(0,\cos\lambda,\sin\lambda)$ and $\mathbf v=(0,-v,0)$. The [Coriolis acceleration in local Earth coordinates](../../../../../coriolis-acceleration-in-local-earth-coordinates.md) gives

$$
\boxed{\mathbf F_{\rm cor}=-2m\boldsymbol\Omega\times\mathbf v
=-2m\Omega v\sin\lambda\,\mathbf e_E.}
$$

It is westward in the northern hemisphere, eastward in the southern hemisphere and zero for exactly southward motion at the equator. There is no vertical Coriolis component for this particular [velocity](../../../../../velocity.md).

**Correct steering.** On the desired meridional track, [drag](../../../../../drag-physics.md) has no eastward component because it is antiparallel to the [velocity](../../../../../velocity.md). If the [thrust](../../../../../thrust.md) makes signed angle $\phi$ east of south, its eastward component is $T\sin\phi$. The cross-track [force](../../../../../force-split.md) balance is therefore

$$
T\sin\phi-2m\Omega v\sin\lambda=0,
$$

so

$$
\boxed{\phi=\sin^{-1}\!\left(\frac{2m\Omega v\sin\lambda}{T}\right).}
$$

The argument must have magnitude at most one for this simple thrust-only correction to be feasible. The signed angle changes sign at the equator: correction is east of south in the north and west of south in the south. Thus the phrase “east of south” cannot describe a positive correction throughout the entire flight.

**Wrong-sign correction and the miss distance.** A literally constant [velocity](../../../../../velocity.md) vector cannot develop a cross-track displacement. The physically useful interpretation of the last task is constant speed, with an erroneous lateral steering correction. In the usual leading-track model, [thrust](../../../../../thrust.md) and [drag](../../../../../drag-physics.md) balance along the actual motion, and the applied transverse correction has the correct magnitude but the wrong sign. It therefore reinforces rather than cancels the [Coriolis force](../../../../../coriolis-force.md). Starting at the equator, use the unperturbed southward track $\lambda\simeq-vt/R$, and let $x_E$ be the eastward departure from that track. To first order in the departure,

$$
\ddot x_E=-4\Omega v\sin\lambda
=4\Omega v\sin\frac{vt}{R},\qquad x_E(0)=\dot x_E(0)=0.
$$

There is a factor two relative to uncompensated Coriolis deflection because the wrong correction adds an equal lateral [force](../../../../../force-split.md). Integration gives the [wrong-sign Coriolis steering error](../../../../../wrong-sign-coriolis-steering-error.md),

$$
\dot x_E=4\Omega R\left(1-\cos\frac{vt}{R}\right),\qquad
x_E=4\Omega R\left[t-\frac Rv\sin\frac{vt}{R}\right].
$$

For southern angular distance $\Lambda=16\pi/180=0.27925$, $R=6.4\times10^6\ \mathrm m$ and $v=800/3.6=222.2\ \mathrm{m\,s^{-1}}$, the nominal flight time after the equator is

$$
t_f=\frac{R\Lambda}{v}\simeq8.04\times10^3\ \mathrm s=2.23\ \mathrm h.
$$

Taking $\Omega\simeq2\pi/(86400\ \mathrm s)$ gives

$$
\boxed{x_E(t_f)\simeq\frac{4\Omega R^2}{v}(\Lambda-\sin\Lambda)
\simeq1.94\times10^5\ \mathrm m,
\quad\text{about }200\ \mathrm{km\ east}.}
$$

The small-latitude approximation $\sin(vt/R)\simeq vt/R$ gives $\ddot x_E\simeq4\Omega v^2t/R$ and $x_E\simeq2\Omega v^2t^3/(3R)$, or $1.95\times10^5\ \mathrm m$, confirming the scale and direction.

This is an estimate under an explicit steering model, not an exact trajectory forced by the wording. For example, retaining spherical transport of the local axes while still linearizing in the cross-track motion gives, with $s=-\lambda$, $\dot u-(v/R)u\tan s=4\Omega v\sin s$. Consequently $u\cos s=2\Omega R\sin^2s$ and the longitude departure is $\Delta\ell=2\Omega R(\tan\Lambda-\Lambda)/v$. The distance along the destination parallel is then $R\cos\Lambda\,\Delta\ell\simeq1.93\times10^5\ \mathrm m$. Corrections from the changed track and a more detailed control law are not fixed by the problem. If “keeps the [velocity](../../../../../velocity.md) constant” instead means the full vector, the pilot would need an additional compensating [force](../../../../../force-split.md) and there would be no miss; if [thrust](../../../../../thrust.md) is kept at a specified geographical bearing despite drift, its along-track component and lateral [drag](../../../../../drag-physics.md) must also be modelled.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
