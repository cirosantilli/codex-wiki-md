<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

On the [surface of revolution](../../../../../../surface-of-revolution.md), a [normal vector](../../../../../../normal-vector.md) is proportional to $-H'(r)\mathbf e_r+\mathbf e_z$. Thus the [normal force](../../../../../../normal-force.md) and [gravity](../../../../../../gravity.md) have no $\mathbf e_\theta$ component. The $\mathbf e_\theta$ component of [Newton's second law](../../../../../../newton-s-second-law.md), using the given [linear drag](../../../../../../linear-drag.md) force, is

$$
m(r\ddot\theta+2\dot r\dot\theta)=-\alpha r\dot\theta.
$$

Multiplication by $r$ therefore gives

$$
\boxed{\dot h=-\frac\alpha m h,\qquad h(t)=h_0e^{-\alpha t/m},\qquad\dot\theta(t)=\frac{h_0e^{-\alpha t/m}}{r(t)^2}.}
$$

**The printed target [equation](../../../../../../equation.md) omits the factor $1/m$.** The matching original PDF, page 5, gives both $\mathbf F_D=-\alpha\dot{\mathbf r}$ and $\dot h=-\alpha h$, so this is a source inconsistency. If its $\alpha$ in the target [equation](../../../../../../equation.md) is intended to mean the drag [coefficient](../../../../../../coefficient.md) per unit [mass](../../../../../../mass.md), put $\lambda=\alpha/m$ and write $\dot h=-\lambda h$. Equivalently, if the intended force was $\mathbf F_D=-m\alpha\dot{\mathbf r}$, the requested convention gives

$$
\boxed{h(t)=h_0e^{-\alpha t},\qquad\dot\theta(t)=h_0e^{-\alpha t}/r(t)^2.}
$$

These formulas determine $\dot\theta$ once $r(t)$ is known; they do not assume a constant [radius](../../../../../../radius.md).

## ↑ Ancestors (12)

1. [a](../a.md)
2. [5](../../5.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
