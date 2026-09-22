<h1 id="38b/solution">Solution</h1>

↑ **Parent:** [38B](../38b.md)

A plane wave in the rest frame of the medium has phase $\mathbf k\cdot\mathbf x-\Omega_0(\mathbf k)t$. Under the [Galilean transformation](../../../../../galilean-transformation.md) $\mathbf x'=\mathbf x-\mathbf U t$, this becomes $\mathbf k\cdot\mathbf x'-[\Omega_0(\mathbf k)-\mathbf U\cdot\mathbf k]t$. Therefore

$$
\boxed{\omega=\Omega_0(\mathbf k)-\mathbf U\cdot\mathbf k,\qquad\mathbf c_g=\nabla_k\Omega_0-\mathbf U.}
$$

Here $\mathbf c_g$ is the [group velocity](../../../../../group-velocity.md) in the moving frame.

For [acoustic waves](../../../../../acoustic-wave.md), $\Omega_0=c_0|\mathbf k|$ and take $\mathbf U=Mc_0\mathbf e_x$. A steady wave has $\omega=0$, requiring $\cos\beta=1/M$, where $\beta$ is the angle of $\mathbf k$ to the flight direction. Its ray velocity is $c_0\widehat{\mathbf k}-Mc_0\mathbf e_x$, with backward component $-c_0(M^2-1)/M$ and transverse magnitude $c_0\sqrt{M^2-1}/M$. Thus the angle $\theta$ of the ray to the backward flight direction obeys

$$
\tan\theta=\frac1{\sqrt{M^2-1}},\qquad\boxed{\theta=\sin^{-1}(1/M).}
$$

The axial symmetry gives the [Mach cone](../../../../../mach-cone.md) behind the aircraft.

For unsteady emitted disturbances, all ray velocities lie on the sphere $\mathbf c_g=-\mathbf U+c_0\widehat{\mathbf k}$. Since $M>1$, the origin lies outside this velocity sphere and its tangent cone has exactly the same semi-angle. All other rays are strictly inside the cone. Equivalently a signal emitted $\tau$ time units ago has a wavefront sphere centered at $-\mathbf U\tau$ with radius $c_0\tau$; these spheres are enclosed by their Mach-cone envelope. Consequently the unsteady wavefield is confined to the cone's interior, with the steady envelope on its boundary.

For [capillary waves](../../../../../capillary-wave.md) put $a=\sqrt{T/\rho}$, so $\Omega_0=ak^{3/2}$. The positive-frequency steady condition is $a\sqrt k=U\cos\beta$, requiring $\cos\beta>0$. Then

$$
\nabla_k\Omega_0=\tfrac32a\sqrt k(\cos\beta,\sin\beta),
$$

and

$$
\boxed{\mathbf c_g=U\left(\tfrac32\cos^2\beta-1,\ \tfrac32\cos\beta\sin\beta\right).}
$$

Its endpoint traces the circle

$$
\left(\frac{c_{gx}}U+\frac14\right)^2+\left(\frac{c_{gy}}U\right)^2=\left(\frac34\right)^2,
$$

since $c_{gx}/U=-1/4+(3/4)\cos2\beta$ and $c_{gy}/U=(3/4)\sin2\beta$. As $\beta$ runs through $(-\pi/2,\pi/2)$ this traces the circle except its leftmost limiting point, corresponding to the zero-wavenumber limit. The circle surrounds the origin, so every direction except the precisely backward axis is attained by a nonzero-wavenumber steady ray; the backward direction is approached as $k\downarrow0$. Thus the closure of the steady ray field extends all around the insect, with no excluded angular sector such as the acoustic Mach-cone exterior.

## ↑ Ancestors (10)

1. [38B](../38b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
