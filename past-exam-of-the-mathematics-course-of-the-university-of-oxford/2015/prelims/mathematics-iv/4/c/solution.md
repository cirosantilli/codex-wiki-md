<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For steady [precession](../../../../../../precession.md) at rate $\Omega$ about the fixed vertical [unit vector](../../../../../../unit-vector.md) $\mathbf k$,

$$
\dot{\mathbf e}=\Omega\mathbf k\wedge\mathbf e,\qquad
\ddot{\mathbf e}=\Omega^2(\cos\alpha\,\mathbf k-\mathbf e).
$$

Consequently $\mathbf e\wedge\ddot{\mathbf e}=\Omega^2\cos\alpha\,\mathbf e\wedge\mathbf k$ and $\dot{\mathbf e}=-\Omega\mathbf e\wedge\mathbf k$. Since the [axial angular velocity of a symmetric top](../../../../../../axial-angular-velocity-of-a-symmetric-top.md) $n$ is constant, substitution in the equation of motion gives

$$
\left(A\Omega^2\cos\alpha-Cn\Omega\right)\mathbf e\wedge\mathbf k
=(\kappa\ell^2-mgh)\mathbf e\wedge\mathbf k.
$$

As $0<\alpha<\pi/2$, the [cross product](../../../../../../cross-product.md) can be cancelled. For a specified axial spin, the required value is

$$
\boxed{\kappa=\frac{mgh+A\Omega^2\cos\alpha-Cn\Omega}{\ell^2}.}
$$

The corresponding total [angular velocity](../../../../../../angular-velocity.md) is

$$
\boldsymbol\omega=\Omega\mathbf k+(n-\Omega\cos\alpha)\mathbf e.
$$

If the stated [angular velocity](../../../../../../angular-velocity.md) $\Omega\mathbf k$ is the total [angular velocity](../../../../../../angular-velocity.md) of the top, then $n=\Omega\cos\alpha$ and the requested value specializes to

$$
\boxed{\kappa=\frac{mgh+(A-C)\Omega^2\cos\alpha}{\ell^2}.}
$$

This specialization permits a direct check: $\mathbf L_Q=A\Omega\mathbf k+(C-A)\Omega\cos\alpha\,\mathbf e$, whose time [derivative](../../../../../../derivative.md) is $(A-C)\Omega^2\cos\alpha\,\mathbf e\wedge\mathbf k$, exactly the required [torque](../../../../../../torque.md). The first formula keeps the separate axial spin explicit when $\Omega$ is understood as the rate of [precession](../../../../../../precession.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
