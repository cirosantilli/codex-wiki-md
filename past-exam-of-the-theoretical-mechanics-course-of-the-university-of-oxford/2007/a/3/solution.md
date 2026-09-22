<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Scale lateral distance with $L$, transverse distance with $h$, lateral [velocity](../../../../velocity.md) with $U$, and the normal [velocity](../../../../velocity.md) with $Uh/L$. Balancing lateral [pressure](../../../../pressure-split.md) force with transverse viscous stress gives [pressure](../../../../pressure-split.md) scale $\mu UL/h^2$. The ratio of inertia to that stress is $Uh^2/(\nu L)$, while lateral viscous [derivatives](../../../../derivative.md) are smaller by $(h/L)^2$. The two stated smallness conditions therefore reduce the lateral equations to $\mu u_{zz}=p_x$, $\mu v_{zz}=p_y$. The normal component of [balance of linear momentum](../../../../balance-of-linear-momentum.md) gives $p_z=0$ at leading order; continuity remains $u_x+v_y+w_z=0$. The no-slip, impermeable rigid plates require $u=v=w=0$ at both plate surfaces.

Integrating with those boundary values gives

$$
(u,v)=-\frac{z(h-z)}{2\mu}\nabla p,\qquad
\boxed{\bar u=-K\nabla p,\quad K=\frac{h^2}{12\mu}.}
$$

Depth-integrated continuity has no normal boundary flux, so $\nabla\cdot\bar u=0$ and $\boxed{\nabla^2p=0}$ away from the injection point.

Neglecting [surface tension](../../../../surface-tension-split.md), the [fluid free boundary](../../../../fluid-free-boundary.md) has $p=p_{\rm ext}$, and its normal [velocity](../../../../velocity.md) is the fluid [velocity](../../../../velocity.md): $\dot R=\bar u_r(R)$. Any constant [capillary pressure](../../../../capillary-pressure.md) for a circular interface can instead be included in that spatially uniform boundary [pressure](../../../../pressure-split.md). Conservation of injected volume gives $2\pi rh\bar u_r=Q$. Hence

$$
\boxed{\bar u_r=\frac{Q}{2\pi hr},\quad
R^2=R_0^2+\frac{Qt}{\pi h},\quad
p(r,t)=p_{\rm ext}+\frac{6\mu Q}{\pi h^3}\log\frac{R(t)}r.}
$$

The logarithmic [pressure](../../../../pressure-split.md) singularity represents the ideal [point source](../../../../point-source.md), which in a physical cell is replaced by a finite inlet. The formula is an exact radial solution of the depth-averaged model for either sign of $Q$, while $R^2>0$.

Its robustness differs sharply between the signs. With viscous fluid inside a much less viscous exterior, injection displaces the less viscous phase and is stabilizing; suction draws the exterior into the viscous region and is prone to fingering. One can see this directly without relying on a slogan. Write the boundary as $R+a_n\cos n\theta$ and its regular [pressure](../../../../pressure-split.md) [perturbation](../../../../perturbation.md) as $b_nr^n\cos n\theta$. Linearizing the constant-[pressure](../../../../pressure-split.md) condition gives $\delta p(R)=-a_np_0'(R)=a_nQ/(2\pi hKR)$. The [perturbation](../../../../perturbation.md) radial [velocity](../../../../velocity.md) is then $-na_nQ/(2\pi hR^2)$, and evaluation of the base [velocity](../../../../velocity.md) at the displaced boundary adds $-a_nQ/(2\pi hR^2)$. Thus

$$
\boxed{\dot a_n=-\frac{(n+1)Q}{2\pi hR^2}a_n.}
$$

Modes decay for injection and grow for suction. Accordingly the suction circle is a mathematically possible symmetric solution but generally an unstable prediction, failing before its formal collapse in a perturbed experiment. This is [Stability of an interior Hele-Shaw blob under injection and suction](../../../../stability-of-an-interior-hele-shaw-blob-under-injection-and-suction.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
