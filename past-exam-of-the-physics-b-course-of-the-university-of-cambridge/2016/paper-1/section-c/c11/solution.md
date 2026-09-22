<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

For a body-fixed [mass](../../../../../mass.md) element at position $\mathbf r$ relative to the fixed tip, $\mathbf v=\boldsymbol\omega\times\mathbf r$. Therefore

$$
\mathbf L=\int\mathbf r\times(\boldsymbol\omega\times\mathbf r)\,dm=\mathsf I\boldsymbol\omega,\qquad I_{ij}=\int(r^2\delta_{ij}-r_ir_j)\,dm.
$$

The [inertia tensor](../../../../../inertia-tensor.md) is real symmetric. Its orthogonal [eigenvectors](../../../../../eigenvector.md) define [principal axes](../../../../../principal-axis.md) and its [eigenvalues](../../../../../eigenvalue.md) are [principal moments of inertia](../../../../../principal-moment-of-inertia.md). [angular momentum](../../../../../angular-momentum.md) is parallel to [angular velocity](../../../../../angular-velocity.md) when rotation is along a [principal axis](../../../../../principal-axis.md), but generally not for arbitrary rotation.

Write $\mathbf n=\hat{\mathbf e}_3$ and $s=I_3\omega_3$. Axial symmetry gives $\mathbf L=I_1\boldsymbol\omega+(I_3-I_1)\omega_3\mathbf n$. Since $\dot{\mathbf n}=\boldsymbol\omega\times\mathbf n$, the vector triple-product identity gives $\mathbf n\times\dot{\mathbf n}=\boldsymbol\omega-\omega_3\mathbf n$. Hence

$$
\boxed{\mathbf L=I_1\mathbf n\times\dot{\mathbf n}+s\mathbf n.}
$$

Differentiate in the [inertial frame](../../../../../inertial-frame.md), using constant $s$ and $\dot{\mathbf n}\times\dot{\mathbf n}=0$. The gravitational [torque](../../../../../torque.md) about the fixed tip is $(\ell\mathbf n)\times(-mg\hat{\mathbf z})$, yielding the [symmetry-axis equation of a heavy symmetric top](../../../../../symmetry-axis-equation-of-a-heavy-symmetric-top.md):

$$
\boxed{s\dot{\mathbf n}+I_1\mathbf n\times\ddot{\mathbf n}=-mg\ell\mathbf n\times\hat{\mathbf z}.}
$$

The tip reaction exerts no moment about that tip.

For steady precession, $\mathbf n=(\sin\theta\cos\Omega_Pt,\sin\theta\sin\Omega_Pt,\cos\theta)$. At azimuth zero, put $s_\theta=\sin\theta$ and $c_\theta=\cos\theta$. Then $\dot{\mathbf n}=(0,\Omega_Ps_\theta,0)$, $\ddot{\mathbf n}=(-\Omega_P^2s_\theta,0,0)$, and the $y$ component gives $s\Omega_Ps_\theta-I_1\Omega_P^2s_\theta c_\theta=mg\ell s_\theta$. For a nonvertical axis this becomes

$$
I_1\cos\theta\,\Omega_P^2-s\Omega_P+mg\ell=0,
$$



$$
\boxed{\Omega_P=\frac{I_3\omega_3\pm\sqrt{I_3^2\omega_3^2-4mg\ell I_1\cos\theta}}{2I_1\cos\theta}.}
$$

Real steady branches require a nonnegative discriminant. In particular, for a top pointing above the horizontal there is a spin threshold for these fixed-angle solutions. At $\cos\theta=0$ use the quadratic's linear limit $\Omega_P=mg\ell/s$, rather than dividing by zero. For a vertical axis, azimuth does not describe a physical conical motion and the division by $\sin\theta$ is inappropriate.

For rapid positive spin $s$ with $s^2\gg4mg\ell I_1\cos\theta$, the [slow and fast steady precession](../../../../../slow-and-fast-steady-precession.md) roots are

$$
\boxed{\Omega_{\rm slow}\simeq\frac{mg\ell}{s},\qquad \Omega_{\rm fast}\simeq\frac{s}{I_1\cos\theta}-\frac{mg\ell}{s}.}
$$

The approximation assumes a nonsingular fixed inclination. For $g=0$, the quadratic instead gives **$\Omega_P=0$ or $\Omega_P=s/(I_1\cos\theta)$**. The zero branch has a stationary symmetry axis and pure axial spin. On the other branch [angular momentum](../../../../../angular-momentum.md) is constant and parallel or antiparallel to the chosen $z$ axis; $L_z=I_1\Omega_P$ and $s=L_z\cos\theta$. This is torque-free precession in space, not the different rate at which transverse components rotate in body coordinates.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
