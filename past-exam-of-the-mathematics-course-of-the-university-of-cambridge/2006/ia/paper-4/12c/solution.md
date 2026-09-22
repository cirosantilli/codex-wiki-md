<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

With the prescribed magnetic-only [Lorentz force](../../../../../lorentz-force.md) $m\ddot{\mathbf r}=q\dot{\mathbf r}\times\mathbf B$, the component equations are

$$
\boxed{\ddot x=\frac qm B_z(t)\dot y,\qquad
\ddot y=-\frac qm B_z(t)\dot x,\qquad
\ddot z=0.}
$$

Differentiate the squared planar speed:

$$
\frac d{dt}(\dot x^2+\dot y^2)
=2\dot x\ddot x+2\dot y\ddot y=0.
$$

Thus $V=\sqrt{\dot x^2+\dot y^2}$ is constant, since the [Lorentz force](../../../../../lorentz-force.md) is perpendicular to the velocity.

For $V>0$, introduce the velocity angle $\theta$ by $\dot x=V\cos\theta$, $\dot y=V\sin\theta$. The two planar equations imply $\dot\theta=-qB_z(t)/m$. Therefore the [velocity rotation in a time-dependent axial magnetic field](../../../../../velocity-rotation-in-a-time-dependent-axial-magnetic-field.md) has phase

$$
\theta(t)=\phi-\frac qm\int_0^t B_z(s)\,ds.
$$

Equivalently, the complex velocity satisfies $\frac d{dt}(\dot x+i\dot y)=-iqB_z(t)(\dot x+i\dot y)/m$, giving the same integrated phase. Integrating the velocities and $\ddot z=0$ proves

$$
\boxed{\begin{aligned}
x(t)&=x_0+V\int_0^t\cos\left(\phi-\frac qm\int_0^{t'}B_z(s)\,ds\right)\,dt',\\
y(t)&=y_0+V\int_0^t\sin\left(\phi-\frac qm\int_0^{t'}B_z(s)\,ds\right)\,dt',\\
z(t)&=z_0+v_z t.
\end{aligned}}
$$

The constants $x_0,y_0,z_0$ are the initial position coordinates, $v_z$ is the constant velocity parallel to the field, $V\geq0$ is the initial planar speed, and $\phi$ is the initial planar-velocity direction modulo $2\pi$. Together they specify the initial position and velocity. If $V=0$, the planar position stays fixed and the angle $\phi$ is immaterial.

For $B_z(t)=\beta t$, the inner integral gives $\theta(t)=-at^2+\phi$, with $a=q\beta/(2m)>0$. Under the specified initial data,

$$
x(t)=\int_0^t\cos(as^2)\,ds,\qquad
y(t)=-\int_0^t\sin(as^2)\,ds,\qquad z(t)=0.
$$

Rescale $u=\sqrt a\,s$. The given [Fresnel integrals](../../../../../fresnel-integral.md) then give

$$
x(\infty)=\frac1{\sqrt a}\sqrt{\frac\pi8}
=\sqrt{\frac{\pi m}{4q\beta}},\qquad
y(\infty)=-\sqrt{\frac{\pi m}{4q\beta}}.
$$

Hence the limiting position is

$$
\boxed{\mathbf r(\infty)=\sqrt{\frac{\pi m}{4q\beta}}\,(1,-1,0).}
$$

The negative $y$ coordinate follows from clockwise rotation of planar velocity for positive charge and positive $B_z$. The position converges through cancellation of increasingly rapid oscillations; its convergence does not mean the constant planar speed tends to zero.

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
