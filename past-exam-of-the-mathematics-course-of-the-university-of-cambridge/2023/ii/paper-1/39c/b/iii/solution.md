<h1 id="39c/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [polar shear stress in a Newtonian fluid](../../../../../../../polar-shear-stress-in-a-newtonian-fluid.md) is

$$
\sigma_{r\theta}
=\mu\left[
 r\frac\partial{\partial r}\left(\frac{u_\theta}{r}\right)
+\frac1r\frac{\partial u_r}{\partial\theta}
\right].
$$

On $r=a$, no slip holds for every $\theta$, so $u_\theta=0$ and $\partial_\theta u_r=0$. Therefore

$$
\sigma_{r\theta}(a,\theta)
=\mu\,\partial_ru_\theta(a,\theta)
=-\mu\psi_{rr}(a,\theta).
$$

Differentiating the solution from part (ii) gives

$$
\psi_{rr}(a,\theta)=\gamma-2\gamma\cos2\theta,
$$

and hence

$$
\boxed{
\sigma_{r\theta}(a,\theta)
=-\mu\gamma+2\mu\gamma\cos2\theta
}.
$$

The moment arm and line element are both $a$, so the torque exerted by the fluid on the disk per unit axial length is

$$
\begin{aligned}
\mathcal T_z
&=a^2\int_0^{2\pi}\sigma_{r\theta}(a,\theta)\,d\theta\\
&=\boxed{-2\pi\mu\gamma a^2}.
\end{aligned}
$$

For $\gamma>0$ the negative sign denotes the clockwise sense of the ambient shear rotation. This agrees with the [hydrodynamic torque on a fixed disk in planar shear](../../../../../../../hydrodynamic-torque-on-a-fixed-disk-in-planar-shear.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [39C](../../../39c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
