<h1 id="36e/solution">Solution</h1>

↑ **Parent:** [36E](../36e.md)

In the thin-current approximation, vertical momentum balance is hydrostatic: $p=p_{\rm atm}+\rho g(h-z)$. Neglect inertia and radial viscous derivatives compared with the vertical ones. The radial [Stokes equation](../../../../../stokes-equation.md) is $\mu u_{zz}=p_r=\rho gh_r$, with no slip at $z=0$ and zero tangential stress $u_z=0$ at $z=h$. Integration gives

$$
\boxed{u(r,z,t)=-\frac{\rho g}{\mu}h_r\left(hz-\frac{z^2}{2}\right).}
$$

Its depth-integrated radial flux is $Q_r=\int_0^hu\,dz=-\rho gh^3h_r/(3\mu)$. Axisymmetric [mass conservation](../../../../../mass-conservation.md) $h_t+r^{-1}\partial_r(rQ_r)=0$ therefore gives

$$
\boxed{h_t=\frac\beta r\partial_r(rh^3h_r),\qquad\beta=\frac{\rho g}{3\mu}.}
$$

The remaining conditions are conserved [volume](../../../../../volume.md) $2\pi\int_0^{R(t)}rh\,dr=V$, regularity and zero radial flux at the center, $h(R(t),t)=0$, zero thickness outside the front, and the initially concentrated [volume](../../../../../volume.md) at the origin. The advancing edge obeys $R'=\lim_{r\uparrow R}Q_r/h$ when this limit exists. One must not impose a finite zero slope at this compact-support edge.

Put $h=t^aF(rt^{-b})$ with dimensional factors to be restored. Constant [volume](../../../../../volume.md) gives $a+2b=0$, while balancing the equation gives $a-1=4a-2b$. Hence $a=-1/4,b=1/8$. In normalized similarity variables $\eta=r/(\beta V^3t)^{1/8}$ and $h=V^{1/4}(\beta t)^{-1/4}F(\eta)$, the equation becomes

$$
-\frac14F-\frac18\eta F'=\frac1\eta(\eta F^3F')'.
$$

Multiplying by $\eta$ and integrating from the regular center yields $\eta F^3F'=-\eta^2F/8$. Where $F>0$, this integrates to $F^3=3(\eta_0^2-\eta^2)/16$. Restoring physical variables gives

$$
\boxed{h(r,t)=\left[\frac3{16\beta t}(R(t)^2-r^2)\right]^{1/3}\quad(0\leq r\leq R(t)),}
$$

with zero thickness outside. Write $h=A(t)(1-r^2/R^2)^{1/3}$. Its [volume](../../../../../volume.md) is $3\pi AR^2/4$, so $A=4V/(3\pi R^2)$. Combining this with $A^3=3R^2/(16\beta t)$ gives

$$
\boxed{R(t)=\left(\frac{1024\beta V^3t}{81\pi^3}\right)^{1/8}.}
$$

The center height scales as $t^{-1/4}$, while the front scales as $t^{1/8}$. The ideal profile has a singular slope at the edge; microscopic contact-line physics is excluded from the lubrication model, which applies to the sufficiently spread bulk current.

## ↑ Ancestors (10)

1. [36E](../36e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
