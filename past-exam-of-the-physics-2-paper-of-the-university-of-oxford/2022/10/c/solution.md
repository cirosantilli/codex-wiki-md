<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define positive $\alpha$ by the [right-hand rule](../../../../right-hand-rule.md) about $+x$, starting from the loop in the $x$-$y$ plane at $\alpha=0$. Its [magnetic dipole moment](../../../../magnetic-dipole-moment.md) becomes

$$
\mathbf m(\alpha)=m(0,-\sin\alpha,\cos\alpha),\qquad m=I\pi a^2.
$$

The corresponding $x$ component of [magnetic dipole torque](../../../../magnetic-dipole-torque.md) is $\tau_x=-m(B_z\sin\alpha+B_y\cos\alpha)$. Integrating $\tau_x=-dE/d\alpha$ gives the mechanical [magnetic dipole potential energy](../../../../magnetic-dipole-potential-energy.md)

$$
E=-\mathbf m\cdot\mathbf B=m(B_y\sin\alpha-B_z\cos\alpha),
$$

where the arbitrary additive constant is chosen as zero. Set $B_\perp=\sqrt{B_y^2+B_z^2}$. For $B_\perp>0$, a positive-amplitude form is

$$
\boxed{E=E_0\cos(\alpha-\alpha_0),\qquad E_0=mB_\perp,\qquad
\cos\alpha_0=-\frac{B_z}{B_\perp},\quad \sin\alpha_0=\frac{B_y}{B_\perp}.}
$$

Equivalently, $\alpha_0=\operatorname{atan2}(B_y,-B_z)$ modulo $2\pi$. With this positive choice, minimum [potential energy](../../../../potential-energy.md) occurs at $\alpha=\alpha_0+\pi$, where the rotating [magnetic dipole moment](../../../../magnetic-dipole-moment.md) aligns with the projection of $\mathbf B$ into the $y$-$z$ plane. If $B_y=B_z=0$, the allowed [torque](../../../../torque.md) vanishes, $E_0=0$ and $\alpha_0$ is arbitrary. Holding [electric current](../../../../electric-current.md) constant includes exchange with its supply; differentiating only the isolated loop's stored [magnetic energy](../../../../magnetic-energy.md) would not give the appropriate mechanical [potential energy](../../../../potential-energy.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
