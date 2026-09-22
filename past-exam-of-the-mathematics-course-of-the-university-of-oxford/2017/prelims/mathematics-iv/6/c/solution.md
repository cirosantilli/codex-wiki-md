<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

Put $\lambda=\omega^2-g/a>0$. The zero value of the [first integral](../../../../../../first-integral.md) in [b](../b.md) gives

$$
\boxed{\left(1+\frac{r^2}{a^2}\right)\dot r^2=\lambda r^2.}
$$

At the endpoint $r=a$, this gives $\dot r^2=\lambda a^2/2$. The absolute [speed](../../../../../../speed.md) includes radial, azimuthal and vertical components. Since $\dot z=\dot r$ there,

$$
|\mathbf v|^2=\dot r^2+(a\omega)^2+\dot z^2
=2\dot r^2+a^2\omega^2=a^2\left(2\omega^2-\frac ga\right).
$$

Hence the limiting exit [speed](../../../../../../speed.md) is

$$
\boxed{|\mathbf v|=a\sqrt{2\omega^2-\frac ga}.}
$$

There is a small [initial condition](../../../../../../initial-condition.md) qualification in the wording. The exact [initial conditions](../../../../../../initial-condition.md) $r=\dot r=0$ give the stationary solution forever, by [Picard-Lindelöf theorem](../../../../../../picard-lindelof-theorem.md). The displayed zero-[first integral](../../../../../../first-integral.md) moving branch instead approaches that [unstable equilibrium](../../../../../../unstable-equilibrium.md) as $t\to-\infty$.

For a precise small disturbance, release the bead with zero relative [velocity](../../../../../../velocity.md) at $r=\epsilon>0$. Its [first integral](../../../../../../first-integral.md) is $J=-\lambda\epsilon^2/2$, giving

$$
\left(1+\frac{r^2}{a^2}\right)\dot r^2=\lambda(r^2-\epsilon^2),\qquad
|\mathbf v_{\rm exit}|^2=a^2\left(2\omega^2-\frac ga\right)-\lambda\epsilon^2.
$$

The bead initially accelerates outward and reaches the end. Letting $\epsilon\to0^+$ recovers exactly the stated exit [speed](../../../../../../speed.md). The conserved $J$ is a [Jacobi integral](../../../../../../jacobi-integral.md) associated with the imposed rotation; ordinary [mechanical energy](../../../../../../mechanical-energy.md) need not be conserved because the apparatus driving the wire can do [work](../../../../../../work.md).

## ↑ Ancestors (12)

1. [c](../c.md)
2. [6](../../6.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
