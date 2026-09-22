<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $K=(k^2+m^2)^{1/2}$ and $P=p'/\rho_0$. Acting on the [Fourier mode](../../../../fourier-mode.md), $D_0=-i(\hat\omega-Uk)=-i\omega$. Continuity and horizontal momentum give $u=-mw/k$ and $P=\omega u/k$. The [buoyancy](../../../../buoyancy.md) equation gives $g\rho'/\rho_0=iN^2w/\omega$. Substitution into vertical momentum yields

$$
\boxed{\omega^2=\frac{N^2k^2}{k^2+m^2},\qquad
\hat\omega=Uk\pm\frac{Nk}{K}.}
$$

The two signs describe the two frequency branches; when the [intrinsic frequency](../../../../intrinsic-frequency.md) is required positive, $\omega=N|k|/K$. For a stationary disturbance $\hat\omega=0$, so $\omega=-Uk>0$. With $U>0$ this requires $k<0$ and selects the minus sign, $\hat\omega=Uk-Nk/K$. The stationary dispersion condition is

$$
\boxed{K=\frac NU,\qquad m^2=\frac{N^2}{U^2}-k^2.}
$$

Differentiate the _unconstrained_ dispersion before imposing stationarity. The [stationary mountain-wave group velocity](../../../../stationary-mountain-wave-group-velocity.md) is obtained from the ground-frame dispersion; before imposing stationarity it is

$$
\hat c_{gx}=U-\frac{Nm^2}{K^3},\qquad
\hat c_{gz}=\frac{Nkm}{K^3}.
$$

On the stationary locus this becomes

$$
\boxed{\widehat{\mathbf c_g}=\frac{Uk}{K^2}(k,m),\qquad
\hat c_{gx}=\frac{Uk^2}{K^2},\quad
\hat c_{gz}=\frac{Ukm}{K^2}.}
$$

Differentiating after substituting $K=N/U$ as though all neighbouring modes were stationary would incorrectly erase the frequency gradients.

For upward [energy](../../../../energy-split.md) propagation from the lower boundary, choose $m<0$, since $k<0$ and $\hat c_{gz}>0$. It requires real nonzero $m$, hence

$$
\boxed{0<|k|<N/U\quad\Longleftrightarrow\quad\lambda_x>2\pi U/N.}
$$

The downstream ray inclination above horizontal is

$$
\boxed{\theta=\tan^{-1}\frac{|m|}{|k|}
=\cos^{-1}\frac{U|k|}{N}=\cos^{-1}\frac\omega N.}
$$

It is fixed for a given monochromatic forcing, with the two signs of $m$ giving the upward/downward rays.

**Frame qualification for the requested phase angle:** the normal intrinsic [phase velocity](../../../../phase-velocity.md) is $\mathbf c_p=\omega(k,m)/K^2$. Because $\omega=-Uk$, the boxed stationary [group velocity](../../../../group-velocity.md) is exactly $-\mathbf c_p$: its angle to _intrinsic_ [phase propagation](../../../../phase-velocity.md) is $\pi$, and it is perpendicular to the stationary phase lines. By contrast the intrinsic [group velocity](../../../../group-velocity.md) $\mathbf c_g=\widehat{\mathbf c_g}-U\hat{\mathbf x}$ satisfies $\mathbf c_g\cdot(k,m)=0$, so its angle to intrinsic [phase propagation](../../../../phase-velocity.md) is $\pi/2$. In the ground frame the [phase velocity](../../../../phase-velocity.md) of a strictly stationary pattern is zero and has no nonzero propagation direction. For example $k=-0.6N/U$, $m=-0.8N/U$ gives $\widehat{\mathbf c_g}=(0.36U,0.48U)$ and $\mathbf c_p=(-0.36U,-0.48U)$. These distinctions prevent applying the usual zero-flow perpendicularity rule to two velocities expressed in different frames.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
