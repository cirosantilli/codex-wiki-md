<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let the thermal-wind basic velocity be

$$
\mathbf U=\Lambda z\,\widehat{\mathbf y},
\qquad
\Lambda=\frac{M^2}{f},
$$

so that $fU_z=b_x=M^2$. Assume constant $f,M,N$, hydrostatic perturbations, $y$ independence, and normal modes proportional to $e^{i(kx+mz-\omega t)}$. The linearized equations are

$$
u_t-fv=-p_x,
\qquad
v_t+fu+\Lambda w=0,
\qquad
p_z=b',
$$



$$
b'_t+M^2u+N^2w=0,
\qquad
u_x+w_z=0.
$$

Incompressibility gives $w=-(k/m)u$. Eliminating $v,p,b'$ yields

$$
\boxed{
\omega^2=f^2-2M^2\frac{k}{m}
+N^2\frac{k^2}{m^2}}.
$$

This quadratic in $k/m$ is positive for every orientation precisely when

$$
\boxed{M^4<N^2f^2}.
$$

Otherwise some disturbances grow monotonically through [symmetric instability](../../../../../symmetric-instability.md).

For the stable case, the minimum occurs at

$$
\frac{k}{m}=\frac{M^2}{N^2},
\qquad
\boxed{\omega_{min}^2=f^2-\frac{M^4}{N^2}}.
$$

Constant-phase lines have slope $dz/dx=-k/m=-M^2/N^2$, exactly the slope of the basic isopycnals $M^2x+N^2z=\text{constant}$. The minimum-frequency displacement follows an isopycnal, allowing buoyancy and Coriolis restoring forces to oppose one another. Its frequency is below the inertial frequency $|f|$ of an unstratified rotating fluid.

If $\theta$ is the counter-clockwise angle of the wavevector from the horizontal, $k/m=\cot\theta$, and

$$
\boxed{
\cot\theta=\frac{M^2\pm
\sqrt{M^4+N^2(\omega^2-f^2)}}{N^2}}.
$$

For $\omega^2>f^2$, define $D=[M^4+N^2(\omega^2-f^2)]^{1/2}>M^2$. Taking $k>0$, the incident wave with group velocity down and right has

$$
\cot\theta_i=\frac{M^2+D}{N^2}>0.
$$

A horizontal reflection preserves $k$ and $\omega$ but selects the other vertical wavenumber, so

$$
\boxed{
\cot\theta_r=\frac{M^2-D}{N^2}<0}.
$$

The incident and reflected phase lines have slopes $-(M^2+D)/N^2$ and $(D-M^2)/N^2$, respectively. Their group velocities are perpendicular to these phase lines: the incident ray points down-right and the reflected ray up-right. The isopycnal slope $-M^2/N^2$ lies between the two phase-line orientations.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
