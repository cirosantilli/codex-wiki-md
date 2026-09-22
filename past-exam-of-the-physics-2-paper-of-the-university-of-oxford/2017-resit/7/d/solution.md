<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a steady filamentary [electric current](../../../../electric-current.md) $I$, the [Biot-Savart law](../../../../biot-savart-law.md) is

$$
\boxed{\mathbf B(\mathbf r)=\frac{\mu_0}{4\pi}\int
\frac{I\,d\boldsymbol\ell'\times(\mathbf r-\mathbf r')}{|\mathbf r-\mathbf r'|^3}.}
$$

Here $\mathbf r$ is the observation position, $\mathbf r'$ the source position, $d\boldsymbol\ell'$ points in the direction of positive [electric current](../../../../electric-current.md), and $\mu_0$ is the [vacuum permeability](../../../../vacuum-permeability.md). A circular loop has centre [magnetic field](../../../../magnetic-field-split.md) $\mu_0I/(2r)$: the cross product has magnitude $r\,d\ell'$ and a constant axial direction, and $\int d\ell'=2\pi r$.

Introduce the constant signed [angular velocity](../../../../angular-velocity.md) $\Omega$ about the positive axis. A ring's [electric charge](../../../../electric-charge-split.md) $dq=2\pi\sigma r\,dr$ crosses any radial cut once per rotation, so its [electric current](../../../../electric-current.md) is $dI=\Omega\,dq/(2\pi)=\sigma\Omega r\,dr$. Adding loop contributions yields the [magnetic field of a rotating charged annulus](../../../../magnetic-field-of-a-rotating-charged-annulus.md):

$$
\mathbf B(0)=\hat{\mathbf x}\int_a^b\frac{\mu_0}{2r}\sigma\Omega r\,dr,
\qquad
\boxed{\mathbf B(0)=\frac{\mu_0\sigma\Omega(b-a)}2\hat{\mathbf x}
=\frac{\mu_0Q\Omega}{2\pi(a+b)}\hat{\mathbf x}.}
$$

The direction follows the [right-hand rule](../../../../right-hand-rule.md) for positive [electric charge](../../../../electric-charge-split.md); reversing either $Q$ or $\Omega$ reverses the [magnetic field](../../../../magnetic-field-split.md). The source supplies no rotation rate, so the answer necessarily retains $\Omega$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
