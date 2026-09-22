<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $D=mR^2+\mathcal I_{33}=m(R^2+a^2/2)$. The [angular acceleration](../../../../../../angular-acceleration.md) is constant. The initial rest conditions and $x(0)=\phi(0)=0$ give

$$
\boxed{\phi(t)=-\frac{T(R\cos\alpha-a)}{2D}t^2,\qquad x(t)=\frac{TR(R\cos\alpha-a)}{2D}t^2.}
$$

For the upward rightward pull in the diagram, $0\leq\alpha\leq\pi/2$, the sign of $x(t)$ is the sign of $R\cos\alpha-a$. Consequently **it rolls towards the horizontal pull when $0\leq\alpha<\arccos(a/R)$**. At $\alpha=\arccos(a/R)$ it remains at rest, with balanced [forces](../../../../../../force-split.md) and [torques](../../../../../../torque.md). For $\arccos(a/R)<\alpha\leq\pi/2$, it rolls to the left. In particular **a horizontal pull, $\alpha=0$, makes it roll to the right**, since $R>a$. If other pulling [angles](../../../../../../angle.md) are allowed, the general condition for motion in the same horizontal direction as the pull is $\cos\alpha(R\cos\alpha-a)>0$.

The required [static friction](../../../../../../static-friction.md) at each rail follows from the translational equation:

$$
\boxed{F_{\mathrm{req}}=\frac{T(\mathcal I_{33}\cos\alpha+maR)}{2D}.}
$$

For $0\leq\alpha\leq\pi/2$ it is positive, agreeing with the leftward [force](../../../../../../force-split.md) convention. The assumed [rolling without slipping](../../../../../../rolling-without-slipping.md) is physically possible only if the rails can supply this [force](../../../../../../force-split.md) while maintaining contact. With [coefficient of static friction](../../../../../../coefficient-of-static-friction.md) $\mu_s$, the necessary contact inequalities are

$$
N=\frac{mg-T\sin\alpha}{2}\geq0,\qquad |F_{\mathrm{req}}|\leq\mu_sN.
$$

For the usual pulling range, these become

$$
\boxed{T\sin\alpha<mg,\qquad T(\mathcal I_{33}\cos\alpha+maR)\leq\mu_sD(mg-T\sin\alpha).}
$$

If either fails, the proposed motion requires lift-off or more [static friction](../../../../../../static-friction.md) than the rails provide. Equality $T\sin\alpha=mg$ is also incompatible here: it gives $N=0$ but a nonzero required [friction](../../../../../../friction.md). The question supplies no [coefficient of static friction](../../../../../../coefficient-of-static-friction.md), so it determines the required [friction](../../../../../../friction.md) exactly but gives no numerical slip threshold. If $F$ is regarded as a prescribed [force](../../../../../../force-split.md) rather than an available contact response, it must equal $F_{\mathrm{req}}$ for the [rolling constraint](../../../../../../rolling-constraint.md) to hold.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
