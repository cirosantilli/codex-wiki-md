<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the horizontal [streamfunction](../../../../../stream-function.md) convention $(u,v)=(-\psi_y,\psi_x)$, and set $a=\pi/L$, $k_d^2=f_0^2/(gH_0)$. [Geostrophic balance](../../../../../geostrophic-balance.md) gives $f_0\bar u=-g\bar\eta_y$, hence

$$
\boxed{\bar\eta(y)=\eta_c+\frac{f_0U_0}{ga}\cos ay,\qquad \bar\psi=\frac{g\bar\eta}{f_0}=\psi_c+\frac{U_0}{a}\cos ay.}
$$

The constant is fixed by the total volume or the reference surface height. To obtain [shallow-water quasi-geostrophic potential vorticity](../../../../../shallow-water-quasi-geostrophic-potential-vorticity.md), require a small [Rossby number](../../../../../rossby-number.md), nearly geostrophic horizontal motion and $|\eta|/H_0\ll1$. Expanding the exact [shallow-water potential vorticity](../../../../../shallow-water-potential-vorticity.md) gives

$$
\frac{\zeta+f_0}{H_0+\eta}=\frac{f_0}{H_0}+\frac1{H_0}\left(\zeta-\frac{f_0\eta}{H_0}\right)+\text{higher orders}.
$$

At leading nontrivial order $\zeta=\nabla_h^2\psi$, so after removing the constant background and multiplying by $H_0$,

$$
\boxed{q=\nabla_h^2\psi-k_d^2\psi,\qquad q_t+J(\psi,q)=0,\quad J(A,B)=A_xB_y-A_yB_x.}
$$

The mean [potential vorticity](../../../../../potential-vorticity.md) and its gradient are

$$
\bar q=-\frac{U_0}{a}(a^2+k_d^2)\cos ay-k_d^2\psi_c,\qquad \boxed{\bar q_y=(a^2+k_d^2)\bar u.}
$$

With $\psi=\bar\psi+\psi'$ and $q=\bar q+q'$, expand the Jacobian. Since both mean fields depend only on $y$, their Jacobian vanishes. The two mixed terms are $\bar u q'_x$ and $v'\bar q_y$, giving

$$
\boxed{q'_t+J(\psi',q')+\bar u q'_x+v'\bar q_y=0,\qquad q'=(\nabla_h^2-k_d^2)\psi'.}
$$

The PDF has this correct mean-advection term; the TeX aid incorrectly inserts a division by $\partial x$.

Drop the quadratic perturbation Jacobian. Freeze $\bar u$ and $\bar q_y$ locally for a short-wave [plane wave](../../../../../plane-wave.md), with $K^2=k^2+l^2$ and $D=K^2+k_d^2$. Then $q'=-D\psi'$, $v'=ik\psi'$, and the [local Rossby-wave dispersion relation in a zonal jet](../../../../../local-rossby-wave-dispersion-relation-in-a-zonal-jet.md) is

$$
\boxed{\omega=k\bar u-\frac{k\bar q_y}{D}=k\bar u\frac{K^2-a^2}{K^2+k_d^2}.}
$$

The intrinsic phase moves against an eastward mean flow because $\omega-k\bar u=-k\bar q_y/D$.

**The printed wavelength bound is not a consequence of these equations.** The local short-wave assumption is $K/a\gg1$, equivalently wavelength $2\pi/K\ll2L$; a particular cutoff $L/2$ is an optional scale-separation criterion, not a universal derived threshold. If one requires the ground-frame phase to follow the mean current, the dispersion relation only gives $K>a$, or wavelength less than $2L$. For example $K=2a,l=0$ has wavelength $L$ and a phase moving with the mean. More decisively, the stationary condition requested next fixes wavelength $2L$, contradicting a bound $L/2$ if both are imposed on the same waves.

For nonzero zonal $k$ and mean velocity, a ground-stationary wave satisfies

$$
\boxed{K=a=\pi/L.}
$$

It has the background length scale, so its existence should not be justified solely by the short-wave approximation. It is nevertheless an exact stationary linear solution of the [Rossby-wave equation for a sheared zonal current](../../../../../rossby-wave-equation-for-a-sheared-zonal-current.md): writing $\psi'=F(y)e^{ikx}$ gives $\bar u[F''-(k^2+k_d^2)F]+\bar q_y F=0$, which reduces to $F''+(a^2-k^2)F=0$. Thus $F=e^{ily}$ with $k^2+l^2=a^2$ works globally. Indeed the total field then has $q=-(a^2+k_d^2)\psi+$ a constant, so its full Jacobian vanishes as well.

Differentiating the local [dispersion relation](../../../../../dispersion-relation.md) gives

$$
\mathbf c_g=\left(\bar u\left[1-\frac{a^2+k_d^2}{D}+\frac{2(a^2+k_d^2)k^2}{D^2}\right],\frac{2\bar u(a^2+k_d^2)kl}{D^2}\right).
$$

On the stationary circle this becomes

$$
\boxed{\mathbf c_g=\frac{2\bar u k}{K^2+k_d^2}(k,l).}
$$

For a purely zonal wavevector, $l=0$, this is the printed expression $\mathbf c_g=2\bar u K^2\hat{\mathbf x}/(K^2+k_d^2)$. With $l\ne0$ the printed expression needs a directional qualification; the general vector is the one above. Here stationarity means $\omega=0$ in the ground frame, not vanishing intrinsic frequency in the moving fluid.

A stationary obstacle can therefore anchor the phase pattern while wave energy travels away from it. The zonal group component has the mean-flow sign, so an eastward jet carries the stationary wave response downstream; tilted wavevectors also carry energy meridionally. This is the usual stationary [Rossby wave](../../../../../rossby-wave.md) wake distinction between fixed phase crests and propagating wave energy.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 79](../../paper-79-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
