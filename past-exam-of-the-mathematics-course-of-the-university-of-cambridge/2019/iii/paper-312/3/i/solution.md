<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A scalar Fourier mode selects one spatial direction, $\hat{\mathbf k}$, and has no transverse vector or tensor polarization. Rotations about $\mathbf k$ therefore leave its temperature and polarization patterns unchanged. Only azimuthal number $m=0$ occurs in the corresponding [spherical harmonic](../../../../../../spherical-harmonic.md) expansion.

Let $\mu=\hat{\mathbf k}\cdot\mathbf e$ and use the paper's convention

$$
\Theta(\eta,\mathbf k,\mathbf e)
=\sum_{\ell\geq0}(-i)^\ell\Theta_\ell(\eta,\mathbf k)P_\ell(\mu),
$$

which omits the $(2\ell+1)$ factor used in some other definitions of the [photon temperature multipole](../../../../../../photon-temperature-multipole.md). In Fourier space the transport term is $ik\mu\Theta$. The [Legendre polynomial recurrence relation](../../../../../../legendre-polynomial-recurrence-relation.md) makes its coefficient at multipole $\ell$ equal to

$$
k\left(\frac{\ell+1}{2\ell+3}\Theta_{\ell+1}
-\frac{\ell}{2\ell-1}\Theta_{\ell-1}\right).
$$

The gravitational time derivative is purely monopolar, and the potential gradient and baryon velocity are dipolar. [Thomson scattering](../../../../../../thomson-scattering.md) removes the monopole from its relaxation term and adds the quadrupole polarization correction. Thus the [photon Boltzmann hierarchy](../../../../../../photon-boltzmann-hierarchy.md) is

$$
\boxed{
\begin{aligned}
\dot\Theta_\ell+
k\left(\frac{\ell+1}{2\ell+3}\Theta_{\ell+1}
-\frac{\ell}{2\ell-1}\Theta_{\ell-1}\right)
={}&-\dot\tau\left[
(\delta_{\ell0}-1)\Theta_\ell-\delta_{\ell1}v_b
+\frac{\delta_{\ell2}}{10}(\Theta_2-\sqrt6E_2)\right]\\
&+\delta_{\ell0}\dot\phi+\delta_{\ell1}k\psi.
\end{aligned}}
$$

The $\ell=0$ term containing $\Theta_{-1}$ is understood as zero.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
