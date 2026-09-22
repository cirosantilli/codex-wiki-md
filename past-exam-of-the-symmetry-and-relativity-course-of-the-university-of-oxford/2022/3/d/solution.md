<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathbf v_1=(c/2,0,0)$ and $\mathbf v_2=(c/(2\sqrt2),c/(2\sqrt2),0)$ in A. Each has [Lorentz factor](../../../../lorentz-factor.md) $g=2/\sqrt3$. The relative [Lorentz factor](../../../../lorentz-factor.md) of $S_2$ in the rest frame of $S_1$ follows from their [four-velocity](../../../../four-velocity.md) [tensor contraction](../../../../tensor-contraction.md):

$$
\Gamma=-\frac{U_1\cdot U_2}{c^2}
=g^2\left(1-\frac{\mathbf v_1\cdot\mathbf v_2}{c^2}\right)
=\frac{8-\sqrt2}{6}.
$$

Let $b=\sqrt{1-\Gamma^{-2}}$ be the relative [speed](../../../../speed.md) divided by $c$. In the rest frame of $S_1$, take $\theta$ between the [photon](../../../../photon.md)'s propagation direction and $S_2$'s [velocity](../../../../velocity.md). The observed [angular frequency](../../../../angular-frequency.md) is the invariant $\omega=-k\cdot U$. Applying it to the emitter, whose rest [angular frequency](../../../../angular-frequency.md) is $\omega_0$, gives $\omega_0=\Gamma\omega_1(1-b\cos\theta)$. Since $\omega_1=\omega_0$,

$$
\boxed{\cos\theta=\frac{1-\Gamma^{-1}}{b}
=\sqrt{\frac{\Gamma-1}{\Gamma+1}}
=\sqrt{\frac{2-\sqrt2}{14-\sqrt2}},\qquad \theta\simeq77.54^\circ.}
$$

This is a [relativistic Doppler effect](../../../../relativistic-doppler-effect.md) calculation using both emitters' and receivers' rest clocks; the time delay of reception introduces no extra factor for constant [velocities](../../../../velocity.md).

For the direction in A, write the [wave four-vector](../../../../four-wavevector.md) as $k^\mu=(\omega_A/c)(1,\mathbf n)$, where $\mathbf n$ is a [unit vector](../../../../unit-vector.md). Equality of the emitted and received [angular frequencies](../../../../angular-frequency.md) gives $k\cdot(U_1-U_2)=0$. Since the two laboratory [Lorentz factors](../../../../lorentz-factor.md) are equal, their time components cancel:

$$
\mathbf n\cdot(\mathbf v_1-\mathbf v_2)=0,
\qquad n_y=(\sqrt2-1)n_x.
$$

Thus the complete answer in three spatial dimensions is

$$
\boxed{\mathbf n=\cos\psi\,\big(\cos(\pi/8),\sin(\pi/8),0\big)+\sin\psi\,(0,0,1),\qquad 0\le\psi<2\pi.}
$$

If propagation is additionally assumed to lie in the stars' motion plane, this reduces to either direction along the internal [angle bisector](../../../../angle-bisector.md), $22.5^\circ$ or $202.5^\circ$ from $+x$. Reflection exchanging the stars' laboratory [velocities](../../../../velocity.md) explains the [angle bisector](../../../../angle-bisector.md) by symmetry. **The source does not specify coplanar propagation or the stars' positions**, so it does not fix the sign or exclude an out-of-plane ray. For example $\mathbf n=(0,0,1)$ gives $\omega_1=\omega_2=g\omega_A$ and satisfies the same no-shift condition. Initial positions can be chosen to make such a ray connect emission and reception. All these possibilities give the same rest-frame $\theta$ above.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
