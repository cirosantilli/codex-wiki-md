<h1 id="12b/solution">Solution</h1>

↑ **Parent:** [12B](../12b.md)

Use an Earth-centred [rotating reference frame](../../../../../rotating-reference-frame.md), with Earth's constant [angular velocity](../../../../../angular-velocity.md) vector $\boldsymbol\omega$. The vectors $\mathbf r$, $\mathbf v$, and $\mathbf a$ are the particle's [position](../../../../../position.md), [velocity](../../../../../velocity.md), and [acceleration](../../../../../acceleration.md) measured in that rotating frame. The vector $\mathbf g$ is the gravitational acceleration due to the actual gravitational force, expressed in the same axes; it excludes the separate [centrifugal acceleration](../../../../../centrifugal-acceleration.md). The remaining term $-2\boldsymbol\omega\times\mathbf v$ is the [Coriolis acceleration](../../../../../coriolis-acceleration.md). A constant rotation axis and an unaccelerated Earth-centred origin account for the absence of an Euler term or a translational-origin term.

For the size estimates, Earth's angular speed is

$$
\omega=\frac{2\pi}{9\times10^4}\approx7.0\times10^{-5}\ {\rm s}^{-1}.
$$

With drop height $H=20\ {\rm m}$, unperturbed [free fall](../../../../../free-fall.md) gives **the fall time**

$$
\boxed{T=\sqrt{\frac{2H}{g}}=2\ {\rm s}},
$$

and final speed $gT=20\ {\rm m\,s}^{-1}$. Thus the gravitational term has size $10\ {\rm m\,s}^{-2}$, the [Coriolis acceleration](../../../../../coriolis-acceleration.md) is at most about $2\omega gT\approx2.8\times10^{-3}\ {\rm m\,s}^{-2}$, and the [centrifugal acceleration](../../../../../centrifugal-acceleration.md) is at most $\omega^2R_0\approx2.9\times10^{-2}\ {\rm m\,s}^{-2}$. These are characteristic sizes $10^1$, $10^{-3}$, and $10^{-2}$ in acceleration units; geometric factors can reduce them, and the Coriolis term is zero at release.

For a suitable approximation to the [rotational deflection of a falling body](../../../../../rotational-deflection-of-a-falling-body.md), take $\mathbf g$ constant over the short fall, start at rest relative to Earth, and use the zeroth-order velocity $\mathbf v^{(0)}(t)=\mathbf g\,t$ inside the small Coriolis term. In the centrifugal term replace $\mathbf r$ by $\mathbf R_0$, because $H/R_0\ll1$. Integrating the resulting acceleration twice, with initial position $\mathbf r_{\rm i}$, gives

$$
\mathbf r(t)\approx\mathbf r_{\rm i}+\frac12\mathbf g\,t^2
-\frac13\boldsymbol\omega\times\mathbf g\,t^3
-\frac12\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf R_0)t^2.
$$

Since $\mathbf r_{\rm i}+\mathbf gT^2/2=\mathbf R_0$, evaluating at the unperturbed fall time yields the printed first-iterate estimate

$$
\boxed{\mathbf R\approx\mathbf R_0
-\frac13\boldsymbol\omega\times\mathbf g\,T^3
-\frac12\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf R_0)T^2}.
$$

The approximation keeps the leading Coriolis contribution and the leading centrifugal contribution enhanced by Earth's large radius. Feeding the Coriolis velocity correction back into the equation produces terms of size $\omega^2gT^4$, smaller than the retained centrifugal displacement by a factor of order $H/R_0$. Replacing $\mathbf r$ by $\mathbf R_0$ in that term has the same relative error. Here $\omega T\approx1.4\times10^{-4}$ and $H/R_0\approx3.3\times10^{-6}$, so both approximations are well controlled. Strictly, the displayed vector is the position at time $T$: its small upward component is removed by the slightly longer actual fall time. That arrival-time correction changes the retained horizontal displacements only at higher order. Thus the horizontal components of the printed estimate give the landing point on the locally flat surface; its vertical component should not be interpreted as a landing above the ground.

Let $\hat{\mathbf e}_E,\hat{\mathbf e}_N,\hat{\mathbf e}_U$ point east, north, and vertically upwards. They form a right-handed basis, with $\hat{\mathbf e}_N\times\hat{\mathbf e}_U=\hat{\mathbf e}_E$. At latitude $\lambda$, in the spherical-Earth approximation,

$$
\boldsymbol\omega=\omega(\cos\lambda\,\hat{\mathbf e}_N+\sin\lambda\,\hat{\mathbf e}_U),
\quad \mathbf g=-g\hat{\mathbf e}_U,\quad
\mathbf R_0=R_0\hat{\mathbf e}_U.
$$

The required [cross products](../../../../../cross-product.md) are

$$
\boldsymbol\omega\times\mathbf g=-\omega g\cos\lambda\,\hat{\mathbf e}_E,
\qquad
\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf R_0)
=\omega^2R_0(\sin\lambda\cos\lambda\,\hat{\mathbf e}_N-\cos^2\lambda\,\hat{\mathbf e}_U).
$$

At $\lambda=45^\circ$, **the northerly and easterly displacements** are therefore

$$
\boxed{\Delta N=-\frac{\omega^2R_0T^2}{4},\qquad
\Delta E=\frac{\omega gT^3}{3\sqrt2}}.
$$

The negative northerly component means a southward displacement. With the supplied values, these are approximately $2.9\ {\rm cm}$ south and $1.3\ {\rm mm}$ east. The eastward effect comes from [Coriolis acceleration](../../../../../coriolis-acceleration.md), while the leading southward effect here comes from [centrifugal acceleration](../../../../../centrifugal-acceleration.md).

## ↑ Ancestors (10)

1. [12B](../12b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
