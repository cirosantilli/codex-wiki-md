<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In the inertial frame the steady convective acceleration is $-R\Omega^2\mathbf e_R$. For a [barotropic fluid](../../../../../barotropic-fluid.md), $\nabla p/\rho=\nabla h$, where $h$ is the [barotropic enthalpy function](../../../../../barotropic-enthalpy-function.md). The equilibrium momentum equation therefore gives

$$
\nabla\left(h+\Phi-\frac12\Omega^2R^2\right)=0,
\qquad\boxed{H=h+\Phi-\frac12\Omega^2R^2=\text{constant}}
$$

on each connected fluid region. Uniform rotation is essential: it makes the [centrifugal acceleration](../../../../../centrifugal-acceleration.md) derivable from the [centrifugal potential](../../../../../centrifugal-potential.md) $-\Omega^2R^2/2$.

The [Cowling approximation](../../../../../cowling-approximation.md) sets the gravitational-potential perturbation to zero while retaining background gravity. The barotropic [pressure](../../../../../pressure.md) force linearizes as $\delta(\nabla p/\rho)=\nabla\delta h$, with $\delta h=p'/\rho=c_s^2\rho'/\rho$. Denote its mode amplitude by $W$. The advective time derivative on a scalar mode is $\partial_t+\Omega\partial_\phi$, so the stated positive-frequency exponential produces $i\sigma$ with $\sigma=\omega+m\Omega$. Linearizing the radial centrifugal term produces $-2\Omega v_\phi$, while linearizing the azimuthal convective term produces $2\Omega v_R$. Thus

$$
i\sigma v_R-2\Omega v_\phi=-W_R,\qquad
i\sigma v_\phi+2\Omega v_R=-imW/R,\qquad
i\sigma v_z=-W_z.
$$

These are the pressure-gradient and [Coriolis acceleration](../../../../../coriolis-acceleration.md) terms in the corotating-frame form. Independently, linearizing [continuity equation](../../../../../continuity-equation.md) gives

$$
\boxed{i\sigma\frac{\rho W}{c_s^2}
=-\frac1R\partial_R(R\rho v_R)-\frac{im\rho v_\phi}R-\partial_z(\rho v_z).}
$$

The equilibrium [mass density](../../../../../density.md) is axisymmetric, so no additional azimuthal background-density derivative appears.

For $\sigma\ne0$ and $D=4\Omega^2-\sigma^2\ne0$, invert the horizontal momentum system:

$$
v_R=-\frac{i}{D}\left(\sigma W_R+\frac{2m\Omega W}R\right),\qquad
v_\phi=\frac1D\left(2\Omega W_R+\frac{m\sigma W}R\right),\qquad
v_z=\frac i\sigma W_z.
$$

Inserting these into the [continuity equation](../../../../../continuity-equation.md), dividing by $i\sigma$ and multiplying by $D$ gives

$$
D\frac{\rho W}{c_s^2}
=\frac1R\partial_R(R\rho W_R)-\frac{m^2\rho W}{R^2}
-\frac D{\sigma^2}\partial_z(\rho W_z)
+\frac{2m\Omega}{R\sigma}\rho_RW.
$$

The two terms proportional to $\rho W_R$ cancel; this cancellation leaves precisely the background-density derivative in the last term. Since $-D/\sigma^2=1-4\Omega^2/\sigma^2$, this is exactly

$$
\boxed{D\frac{\rho W}{c_s^2}
=\frac1R\partial_R(R\rho W_R)-\frac{m^2\rho W}{R^2}
+\left(1-\frac{4\Omega^2}{\sigma^2}\right)\partial_z(\rho W_z)
+\frac{2m\Omega}{R\sigma}\rho_RW.}
$$

The singular frequency cases require the original [velocity](../../../../../velocity.md) equations rather than this inversion.

In the low-frequency [anelastic approximation for a rotating barotropic star](../../../../../anelastic-approximation-for-a-rotating-barotropic-star.md), neglect the left side. Spherical background [mass density](../../../../../density.md) satisfies $\rho_R/R=\rho_z/z$, understood by its smooth limiting form on the equatorial plane. For $W=zR^m$,

$$
\frac1R\partial_R(R\rho W_R)-\frac{m^2\rho W}{R^2}
=mzR^{m-1}\rho_R,\qquad
\partial_z(\rho W_z)=R^m\rho_z.
$$

The remaining equation reduces to

$$
R^m\rho_z\left[m+1+\frac{2m\Omega}\sigma-\frac{4\Omega^2}{\sigma^2}\right]=0.
$$

Writing $q=2\Omega/\sigma$, the bracket factors as $(m+1-q)(q+1)$. The regular desired branch is therefore

$$
\boxed{\sigma=\frac{2\Omega}{m+1},\qquad W=zR^m.}
$$

The other algebraic factor corresponds to $\sigma=-2\Omega$, where the eliminated horizontal system is singular; it is not classified by this pressure-equation inversion. A constant-density background makes the bulk factor identically zero but does not invalidate the displayed solution.

For the regular branch, an explicit [velocity](../../../../../velocity.md) check is particularly informative. Up to a common mode normalization,

$$
(v_R,v_\phi,v_z)=\frac{m+1}{2\Omega}\bigl(-izR^{m-1},\ zR^{m-1},\ iR^m\bigr).
$$

It satisfies $Rv_R+zv_z=0$ and $\nabla\cdot\mathbf v=0$. Thus $\nabla\cdot(\rho\mathbf v)=0$ for every spherical [mass density](../../../../../density.md) profile, directly verifying the anelastic continuity condition. The motion is tangential to spherical shells and is the [sectoral inertial mode of a slowly rotating barotropic star](../../../../../sectoral-inertial-mode-of-a-slowly-rotating-barotropic-star.md). For single-valued azimuthal modes, $m$ is a positive integer. With the source's exponential convention,

$$
\omega=\sigma-m\Omega=-\frac{(m-1)(m+2)}{m+1}\Omega.
$$

For $m\ge2$ the pattern is retrograde relative to the star but prograde in the inertial frame. This is a leading slow-rotation anelastic mode, not an exact solution of the compressible equations whose left-hand term was discarded.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
