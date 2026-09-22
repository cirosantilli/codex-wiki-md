<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

With no electric field, the [Lorentz force](../../../../../lorentz-force.md) is $F=q\dot r\times B\hat z$. The equation from [Newton's second law](../../../../../newton-s-second-law.md) and its first integral are

$$
m\ddot r=qB\dot r\times\hat z,\qquad
\frac{d}{dt}\bigl(\dot r-\omega r\times\hat z\bigr)=0,
\qquad \boxed{\omega=\frac{qB}{m}}.
$$

The [cyclotron frequency](../../../../../cyclotron-frequency.md) is $|\omega|$; the sign of $\omega$ specifies the sense of rotation. Since $\hat x\times\hat z=-\hat y$, the initial data give

$$
\boxed{c=(u+a\omega)\hat y+v\hat z.}
$$

The component equations are $\dot x=\omega y$, $\dot y+\omega x=u+a\omega$ and $\dot z=v$. For $\omega\ne0$, differentiating the first gives

$$
\ddot x+\omega^2x=\omega(u+a\omega),\qquad x(0)=a,\quad\dot x(0)=0.
$$

Solving this [linear differential equation](../../../../../linear-differential-equation.md) and then using $y=\dot x/\omega$ gives

$$
\boxed{r(t)=\left[a+\frac u\omega(1-\cos\omega t)\right]\hat x
+\frac u\omega\sin\omega t\,\hat y+vt\,\hat z.}
$$

The perpendicular projection is a circle of radius $|u/\omega|$ centred at $(a+u/\omega,0)$, the [guiding centre](../../../../../guiding-center.md). The velocity parallel to the [magnetic field](../../../../../magnetic-field.md) stays constant, producing [helical motion in a uniform magnetic field](../../../../../helical-motion-in-a-uniform-magnetic-field.md).

When $a\omega+u=0$, this simplifies to

$$
\boxed{x=a\cos\omega t,\qquad y=-a\sin\omega t,\qquad z=vt.}
$$

Thus the trajectory is a [helix](../../../../../helix.md) about the $z$ axis, with radius $|a|$ and axial advance $2\pi v/|\omega|$ per complete revolution in increasing time. Its projection moves clockwise when viewed from positive $z$ for $\omega>0$. If $v=0$ it is a circle; if $a=0$ it is a straight line along the axis.

<a id="3b/image-helical-trajectory-about-the-magnetic-field-axis-when-a-omega-plus-u-is-zero"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4-magnetic-helix.png)

**[Figure 1](#3b/image-helical-trajectory-about-the-magnetic-field-axis-when-a-omega-plus-u-is-zero). Helical trajectory about the magnetic-field axis when a omega plus u is zero**.

For $\omega=0$, the [Lorentz force](../../../../../lorentz-force.md) vanishes and the solution is instead $r(t)=a\hat x+ut\hat y+vt\hat z$, also the limit of the general formula. The special condition then forces $u=0$.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
