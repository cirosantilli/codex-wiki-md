<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The imposed constraint now fixes $\dot\phi=\omega$, while a torque allows $h=r^2\omega$ to vary as the particle moves radially. The meridional equations become $\ddot r=-\Phi_r+\omega^2r$ and $\ddot z=-\Phi_z$. Hence **$\boxed{\Phi_2=\Phi-\tfrac12\omega^2r^2}$** is the appropriate [effective potential](../../../../../../effective-potential.md). One must not substitute a variable h into the fixed-angular-momentum potential and then differentiate as though h were constant.

For a [point mass](../../../../../../point-mass.md) and nonzero $\omega$, the stationary point is $(r_c,0)$ with $r_c=(GM/\omega^2)^{1/3}$. Its meridional [Hessian matrix](../../../../../../hessian-matrix.md) is

$$
\left.\nabla^2_{r,z}\Phi_2\right|_{(r_c,0)}=\omega^2\begin{pmatrix}-3&0\\0&1\end{pmatrix}.
$$

It is a saddle, at $\Phi_2=-3GM/(2r_c)$. Near it the contours are hyperbolas, with the saddle contour locally tangent to $z=\pm\sqrt3(r-r_c)$, as shown in the right panel. On the equatorial plane the potential tends downward both toward the point mass and at large cylindrical radius; at fixed r it increases as $|z|$ increases. The radial perturbation obeys $\delta\ddot r=3\omega^2\delta r$, while the vertical perturbation obeys $\delta\ddot z=-\omega^2\delta z$. Thus the radial motion has growing and decaying exponential solutions and the vertical motion is oscillatory. For $\omega=0$ no such stationary point exists.

This saddle is the basis of [magnetocentrifugal acceleration](../../../../../../magnetocentrifugal-acceleration.md). A sufficiently strong, open [poloidal magnetic field](../../../../../../poloidal-magnetic-field.md) can enforce approximate corotation with its disc footpoint while allowing motion along the field. If its outward tangent makes angle $\vartheta$ with the vertical, a small distance l along it has $\delta r=l\sin\vartheta$, $\delta z=l\cos\vartheta$. Its leading potential change at a [Keplerian rotation](../../../../../../keplerian-disk.md) footpoint is

$$
\Delta\Phi_2=\frac12\omega^2l^2(\cos^2\vartheta-3\sin^2\vartheta)+O(l^3)=\frac12\omega^2l^2(1-4\sin^2\vartheta)+O(l^3).
$$

The [thirty-degree magnetocentrifugal launching criterion](../../../../../../thirty-degree-magnetocentrifugal-launching-criterion.md) follows: **cold local launching has a downhill quadratic direction when $\boxed{\vartheta>30^\circ}$ from the vertical**. Equality is marginal at quadratic order and depends on higher terms and field-line geometry. The field transmits the torque needed to increase the material's angular momentum; a freely moving particle has no such constraint and instead sees the stable minimum in part (a). The local criterion does not by itself prove global escape or determine the mass loading of a complete magnetohydrodynamic wind.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
