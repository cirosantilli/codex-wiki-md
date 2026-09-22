<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use a local, homogeneous [razor-thin disk approximation](../../../../../razor-thin-disk-approximation.md) in a frame rotating with constant $\Omega$. The unperturbed planar [velocity](../../../../../velocity.md) is zero in this frame, and the large-scale gravitational and centrifugal [forces](../../../../../force.md) balance. Neglect viscosity, magnetic fields, thickness and background gradients across a [wavelength](../../../../../wavelength.md). Take small planar disturbances, with [wavelength](../../../../../wavelength.md) short compared with the [galaxy](../../../../../galaxy-split.md)'s background scale but long enough for a fluid description. The [barotropic closure of a razor-thin disk](../../../../../barotropic-closure-of-a-razor-thin-disk.md) is $P=K\Sigma^\gamma$, with $K$ fixed and a positive derivative

$$
c^2=\left.\frac{dP}{d\Sigma}\right|_0=\frac{\gamma P_0}{\Sigma_0}.
$$

[Solid-body rotation](../../../../../solid-body-rotation.md) has no shear and has [radial epicyclic frequency](../../../../../radial-epicyclic-frequency.md) $\kappa=2|\Omega|$. By rotational symmetry of the local model choose a wavevector along $x$, and write perturbations proportional to $e^{i(kx-\omega t)}$.

Let $\Sigma_1,u,v,\Phi_1$ be the [surface density](../../../../../surface-density-of-a-disk.md), $x$-velocity, $y$-velocity and [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) amplitudes. The linearized [continuity equation](../../../../../continuity-equation.md) and [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) with the [Coriolis force](../../../../../coriolis-force.md) are

$$
-i\omega\Sigma_1+ik\Sigma_0u=0,
\qquad
-i\omega u-2\Omega v=-ik\left(c^2\frac{\Sigma_1}{\Sigma_0}+\Phi_1\right),
\qquad
-i\omega v+2\Omega u=0.
$$

The perturbing [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) solves the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md)

$$
(\partial_z^2-k^2)\Phi_1(z)=4\pi G\Sigma_1\delta(z).
$$

Its decaying solution is proportional to $e^{-|k||z|}$. The jump in its derivative is $-2|k|\Phi_1(0)=4\pi G\Sigma_1$, giving the [razor-thin disk Poisson kernel](../../../../../razor-thin-disk-poisson-kernel.md)

$$
\Phi_1(0)=-\frac{2\pi G\Sigma_1}{|k|}.
$$

Eliminating $v$ from the two momentum equations, and using $\Sigma_1=k\Sigma_0u/\omega$, gives the density-wave branch

$$
\boxed{\omega^2=c^2k^2-2\pi G\Sigma_0|k|+4\Omega^2.}
$$

The complete linear system also has a zero-frequency balanced mode; it is not the growing density-wave branch, and division by $\omega$ in this elimination excludes it. The result is the [uniformly rotating gas-sheet dispersion relation](../../../../../uniformly-rotating-gas-sheet-dispersion-relation.md): [pressure](../../../../../pressure.md) opposes compression at large [wavenumber](../../../../../wavenumber.md), [self-gravity](../../../../../self-gravity.md) promotes compression, and rotation provides epicyclic support.

A mode is exponentially unstable when $\omega^2<0$. With $\Omega=0$ and $c>0$, this occurs at

$$
\boxed{0<|k|<\frac{2\pi G\Sigma_0}{c^2}.}
$$

The uniform $k=0$ perturbation is marginal rather than growing in this local calculation. With $c=0$, rotation fails to stabilize sufficiently short waves:

$$
\boxed{|k|>\frac{2\Omega^2}{\pi G\Sigma_0}.}
$$

These limits show why both [pressure](../../../../../pressure.md) and rotation are needed for stability at all [wavelengths](../../../../../wavelength.md).

For nonzero [pressure](../../../../../pressure.md) and rotation, put $q=|k|$. Complete the square:

$$
\omega^2=c^2\left(q-\frac{\pi G\Sigma_0}{c^2}\right)^2
+4\Omega^2-\frac{(\pi G\Sigma_0)^2}{c^2}.
$$

Its minimum lies at $q_*=\pi G\Sigma_0/c^2$. Thus a growing mode exists precisely when

$$
\boxed{\frac{|\Omega|c}{G\Sigma_0}<\frac\pi2.}
$$

**The printed inequality has the opposite physical meaning: it is the condition for no exponentially growing density wave.** Equality is marginal. In the usual gas [Toomre stability criterion](../../../../../toomre-s-stability-criterion.md), $Q=\kappa c/(\pi G\Sigma_0)=2|\Omega|c/(\pi G\Sigma_0)$, so instability is $Q<1$ and stability is $Q\geq1$. The [unstable wavenumber band of a rotating gas sheet](../../../../../unstable-wavenumber-band-of-a-rotating-gas-sheet.md) is

$$
q_-<|k|<q_+,\qquad
q_\pm=\frac{\pi G\Sigma_0}{c^2}\left(1\pm\sqrt{1-Q^2}\right),
$$

when $Q<1$.

If $\Sigma_0$ and $\Omega\ne0$ remain fixed while $c^2$ decreases slowly, first reach marginality at

$$
c_{\mathrm{crit}}=\frac{\pi G\Sigma_0}{2|\Omega|},\qquad
q_{\mathrm{crit}}=\frac{4\Omega^2}{\pi G\Sigma_0}.
$$

The first [wavelength](../../../../../wavelength.md) to become unstable just below this threshold is the [marginal fragmentation wavelength of a rotating sheet](../../../../../marginal-fragmentation-wavelength-of-a-rotating-sheet.md):

$$
\boxed{\ell_{\mathrm{crit}}=\frac{2\pi}{q_{\mathrm{crit}}}
=\frac{\pi^2G\Sigma_0}{2\Omega^2}
=\frac{2c_{\mathrm{crit}}^2}{G\Sigma_0}.}
$$

Density maxima are separated by approximately this [wavelength](../../../../../wavelength.md). The expected fragment size is of this order; an overdense half-wave has width about $\ell_{\mathrm{crit}}/2$. Linear theory fixes a preferred [wavelength](../../../../../wavelength.md), not an exact nonlinear clump radius or shape. Further cooling shifts the fastest-growing [wavelength](../../../../../wavelength.md) to $2c^2/(G\Sigma_0)$. A rough fragment [mass](../../../../../mass.md) is consequently of order $\Sigma_0\ell_{\mathrm{crit}}^2$, with a geometrical factor depending on the nonlinear fragmentation pattern.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
