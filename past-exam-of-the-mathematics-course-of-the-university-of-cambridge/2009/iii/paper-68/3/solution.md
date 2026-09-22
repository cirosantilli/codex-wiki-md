<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In a [thin disk](../../../../../thin-disk.md) dominated by a central stellar mass, the vertical [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) is harmonic to leading order, so its vertical acceleration is $-\Omega_0^2z$. For a locally isothermal background, $p=c_s^2\rho$ with $c_s$ independent of height. Vertical [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) therefore gives

$$
c_s^2\frac{d\rho}{dz}=-\rho\Omega_0^2z,\qquad
\boxed{\rho(R,z)=\rho(R,0)\exp\left(-\frac{z^2}{2H^2}\right),\quad H=\frac{c_s}{\Omega_0}.}
$$

This is the [isothermal vertical structure in stellar gravity](../../../../../isothermal-vertical-structure-in-stellar-gravity.md). On the upper half of the disk the downward gravity magnitude is $g=\Omega_0^2z>0$; the density profile extends evenly through the midplane.

For an adiabatically displaced parcel kept in [pressure](../../../../../pressure.md) equilibrium, the parcel's logarithmic density gradient is $\gamma^{-1}d\log p/dz$, whereas the environmental density gradient is $d\log\rho/dz$. A small upward displacement $\eta$ consequently produces a density contrast $\delta\rho/\rho=[\gamma^{-1}d\log p/dz-d\log\rho/dz]\eta$. Its [buoyancy](../../../../../buoyancy.md) acceleration is $-g\delta\rho/\rho=-N^2\eta$. Thus the [Brunt–Väisälä frequency](../../../../../buoyancy-frequency.md) is

$$
N^2=g\left(\frac1\gamma\frac{d\log p}{dz}-\frac{d\log\rho}{dz}\right).
$$

Both background gradients equal $-z/H^2$ in the isothermal atmosphere, so

$$
\boxed{N^2=\left(1-\frac1\gamma\right)\frac{z^2}{H^2}\Omega_0^2.}
$$

An isothermal background is therefore stably stratified for adiabatic perturbations with $\gamma>1$, but not buoyant for isothermal perturbations. In applying the adiabatic equation of state to a stratified atmosphere, its proportionality relates Lagrangian parcel changes: $\Delta p=(\gamma p/\rho)\Delta\rho$. Eulerian perturbations generally obey $p'+\eta p_z=(\gamma p/\rho)(\rho'+\eta\rho_z)$ instead. Thus the printed simple proportionality must be interpreted as a parcel relation for the buoyancy calculation. For $\gamma=1$ in this isothermal background, the gradient terms cancel and the Eulerian proportionality holds too.

Now take isothermal perturbations, so $\gamma=1$ and $N^2=0$. The two supplied wave equations reduce to

$$
\xi_z=\omega^2u_z,\qquad
(u_z)_z-\frac z{H^2}u_z+\left(\frac1{c_s^2}-\frac{k^2}{\omega^2-\Omega_0^2}\right)\xi=0.
$$

For the nonsingular oscillatory case $\omega\ne0$ and $\omega^2\ne\Omega_0^2$, substitute $u_z=\xi_z/\omega^2$. With $x=z/H$, the resulting [Hermite differential equation](../../../../../hermite-differential-equation.md) is

$$
\boxed{\xi_{xx}-x\xi_x+\alpha\xi=0,\qquad
\alpha=\frac{\omega^2}{\Omega_0^2}\left(1-\frac{k^2c_s^2}{\omega^2-\Omega_0^2}\right).}
$$

The exceptional frequencies must be treated through the original velocity-[pressure](../../../../../pressure.md) equations rather than division by these factors.

The physical vertical condition is finite perturbation energy when integrated with the Gaussian density. In particular the [pressure](../../../../../pressure.md) contribution is proportional to $\int e^{-x^2/2}|\xi|^2dx$ for nonzero frequency. Generic nonterminating solutions have an exponentially growing component at at least one vertical end and fail this condition; acceptable modes are the terminating [Hermite polynomials](../../../../../hermite-polynomial.md). This is a finite-energy condition, not pointwise boundedness of the velocity in the vanishing-density atmosphere.

To prove the allowed values of $\alpha$, let the nonzero [polynomial](../../../../../polynomial-split.md) have degree $n$ and leading coefficient $a_n$. The highest power in $\xi_{xx}-x\xi_x+\alpha\xi$ has coefficient $(\alpha-n)a_n$. Hence $\alpha=n\in\{0,1,2,\ldots\}$. Conversely, writing $\xi=\sum_j a_jx^j$ gives the recurrence

$$
a_{j+2}=\frac{j-\alpha}{(j+2)(j+1)}a_j.
$$

For $\alpha=n$, choose the parity of $n$ and iterate until the series terminates at degree $n$. Thus all allowed [Hermite vertical modes of an isothermal disk](../../../../../hermite-vertical-mode-of-an-isothermal-disk.md) have

$$
\boxed{\alpha=n,\qquad \xi=C\,\mathrm{He}_n(z/H),}
$$

where $\mathrm{He}_n$ is the [Probabilists' Hermite polynomial](../../../../../probabilists-hermite-polynomial.md). In particular, $\mathrm{He}_0=1$ and $\mathrm{He}_1=x$.

Let $K=kH$ and $s=\omega^2/\Omega_0^2$. Eliminating the denominator for regular modes gives

$$
(s-n)(s-1)=K^2s,\qquad
(\omega^2-n\Omega_0^2)(\omega^2-\Omega_0^2)=k^2c_s^2\omega^2.
$$

For $n=0$, the nonzero-frequency solution is

$$
\boxed{\omega^2=\Omega_0^2(1+K^2)=\Omega_0^2+k^2c_s^2.}
$$

Its [pressure](../../../../../pressure.md) variable is independent of height and $u_z=0$. These are [inertial-acoustic waves](../../../../../inertial-acoustic-wave.md), restored by [epicyclic motion](../../../../../epicyclic-motion.md) and [pressure](../../../../../pressure.md); at short radial [wavelength](../../../../../wavelength.md) they become ordinary [acoustic waves](../../../../../acoustic-wave.md). The multiplied dispersion [polynomial](../../../../../polynomial-split.md) also has $s=0$. This is not an extra oscillatory solution represented by nonzero $\xi$, since $\xi=i\omega p'/\rho$ vanishes at zero frequency for finite [pressure](../../../../../pressure.md) perturbation. The full horizontal equations have a [zero-frequency balanced mode of an axisymmetric disk](../../../../../zero-frequency-balanced-mode-of-an-axisymmetric-disk.md), with no radial velocity and azimuthal [Coriolis acceleration](../../../../../coriolis-acceleration.md) balancing a radial [pressure](../../../../../pressure.md) gradient. It must be recovered without dividing by $\omega$, rather than counted as a propagating wave. At $k=0$, the propagating branch limits to an epicyclic oscillation at $|\omega|=\Omega_0$, another value at which the eliminated form must be interpreted by a limit.

For $n=1$, solve $(s-1)^2=K^2s$. The two branches are

$$
\boxed{\omega_\pm^2=\Omega_0^2\left(1+\frac{K^2}{2}\pm\frac{|K|}{2}\sqrt{K^2+4}\right)
=\frac{\Omega_0^2}{4}\left(\sqrt{K^2+4}\pm|K|\right)^2.}
$$

Both signs of frequency occur on each squared-frequency branch. The upper branch is acoustic in the large-$|K|$ limit, $|\omega_+|\sim |k|c_s$; the lower branch is an [inertial wave](../../../../../inertial-wave.md) with $|\omega_-|\sim\Omega_0/|K|$. At $|K|\ll1$, both frequencies approach $\Omega_0$, reflecting the equality of the radial and [vertical epicyclic frequencies](../../../../../vertical-epicyclic-frequency.md) in a [Keplerian disk](../../../../../keplerian-disk.md). Here $\xi\propto z$, so $u_z=\xi_z/\omega^2$ is independent of height: these modes have a coherent vertical displacement of the disk column, rather than a vertical breathing motion.

For a local non-axisymmetric disturbance proportional to $e^{i(kR+m\phi-\omega t)}$, the material frequency is $\widehat\omega=\omega-m\Omega_0$. In the same local radial-wave approximation, replace $\omega$ by $\widehat\omega$. For $n=1,m=1$, this gives

$$
\boxed{\left[(\omega-\Omega_0)^2-\Omega_0^2\right]^2=k^2c_s^2(\omega-\Omega_0)^2.}
$$

The four frequencies can equivalently be written $\omega/\Omega_0=1\pm(\sqrt{K^2+4}\pm|K|)/2$, with independent choices of the two signs. This is a local [dispersion relation](../../../../../dispersion-relation.md), not a claim that Doppler substitution supplies an exact global non-axisymmetric solution in a differentially rotating disk. The radial-wave ordering neglects azimuthal gradients compared with radial gradients; $|k|R\gg1$ can coexist with $|k|H\ll1$ in a [thin disk](../../../../../thin-disk.md).

Write $w=\omega/\Omega_0$. For the two low inertial-frame frequency branches, $|w|\ll1$, while the material frequency remains near $-\Omega_0$. Expanding the [dispersion relation](../../../../../dispersion-relation.md) gives

$$
(w^2-2w)^2=K^2(w-1)^2,\qquad
4w^2=K^2+\text{higher-order terms}.
$$

Therefore

$$
\boxed{\frac{\omega}{\Omega_0}=\pm\frac12kH+O((kH)^2),\qquad
\frac{d\omega}{dk}\simeq\pm\frac{c_s}{2}.}
$$

For signed $k$, the two leading branches are conventionally labelled by $\pm kH/2$. These are [bending waves of a Keplerian disk](../../../../../bending-wave-of-a-keplerian-disk.md): an $m=1$ vertical displacement varies once around an annulus and corresponds to a small tilt of its orbital plane. A radial variation of the tilt is a warp. **The waves transport the warp radially at group speeds $c_s/2$ in opposite directions.** At zero radial wavenumber their low-frequency limit is a stationary rigid tilt; the apparent slow pattern does not mean that the orbiting gas has slow vertical motion in its own frame.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
