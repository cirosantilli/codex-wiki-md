<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the positive $z$ direction along the sphere's laboratory [velocity](../../../../velocity.md) $v\hat{\mathbf z}$. In its rest frame the far-field fluid velocity is $-v\hat{\mathbf z}$. Therefore the far-field potential is $-vr\cos\theta$. The impermeable sphere imposes $\partial_r\phi=0$ at $r=R$. The monopole coefficient vanishes because the sphere is not a source or sink, and the dipole coefficient follows from the wall condition:

$$
A_1=-v,\qquad B_0=0,\qquad B_1=-\frac{vR^3}{2}.
$$

Thus

$$
\boxed{\phi=-v\left(r+\frac{R^3}{2r^2}\right)\cos\theta+C,\qquad r\ge R.}
$$

The regular exterior [boundary value problem](../../../../boundary-value-problem-split.md) has no forced higher multipoles; uniqueness fixes their coefficients to zero. Differentiating gives

$$
\boxed{u_r=-v\left(1-\frac{R^3}{r^3}\right)\cos\theta,\quad
u_\theta=v\left(1+\frac{R^3}{2r^3}\right)\sin\theta,\quad u_\varphi=0.}
$$

Here $u_\theta$ is the polar [velocity](../../../../velocity.md) component. An equivalent Cartesian form is

$$
\mathbf u=-v\hat{\mathbf z}+\frac{vR^3}{2r^3}\left[3\cos\theta\,\hat{\mathbf r}-\hat{\mathbf z}\right].
$$

Only no-penetration, not no-slip, is appropriate to this ideal inviscid solution. The sphere density $\rho_0$ does not enter the [velocity](../../../../velocity.md) field for an externally prescribed constant speed.[Section 2.3.2, Flow Around a Sphere, potential and impermeable-surface condition; the present far-field velocity has the opposite sign](../../../../fluid-mechanics-by-david-tong.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the flows, fluctuations and complexity course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity course of the University of Oxford](../../../../flows-fluctuations-and-complexity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
