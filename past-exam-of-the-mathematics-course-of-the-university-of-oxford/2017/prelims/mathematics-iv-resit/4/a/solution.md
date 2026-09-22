<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the pivot as origin, with $x$ horizontal and $y$ vertically upward. For the [simple pendulum](../../../../../../simple-pendulum-split.md), put

$$
\mathbf r=\ell(\sin\theta,-\cos\theta),\qquad
\mathbf e_r=(\sin\theta,-\cos\theta),\qquad
\mathbf e_\theta=(\cos\theta,\sin\theta).
$$

The [velocity](../../../../../../velocity.md) and [acceleration](../../../../../../acceleration.md) are

$$
\dot{\mathbf r}=\ell\dot\theta\mathbf e_\theta,\qquad
\ddot{\mathbf r}=\ell\ddot\theta\mathbf e_\theta-\ell\dot\theta^2\mathbf e_r.
$$

The [forces](../../../../../../force-split.md) are the [tension](../../../../../../tension.md) $-T\mathbf e_r$ and [gravity](../../../../../../gravity.md) $(0,-mg)$. Taking the [dot product](../../../../../../dot-product.md) of [Newton's second law](../../../../../../newton-s-second-law.md) with $\mathbf e_\theta$ eliminates the [tension](../../../../../../tension.md) and gives

$$
m\ell\ddot\theta=-mg\sin\theta,
\qquad\boxed{\ell\ddot\theta=-g\sin\theta.}
$$

Near the downward [stable equilibrium](../../../../../../stable-equilibrium.md) $\theta=0$, the [small-angle approximation](../../../../../../small-angle-approximation.md) $\sin\theta\simeq\theta$ gives $\ddot\theta=-(g/\ell)\theta$ to first order. Since $x=\ell\sin\theta\simeq\ell\theta$, its [linearization](../../../../../../linearization.md) is

$$
\boxed{\ddot x=-\frac g\ell x.}
$$

This is [simple harmonic motion](../../../../../../simple-harmonic-motion.md) with [angular frequency](../../../../../../angular-frequency.md) $\sqrt{g/\ell}$; the restoring sign confirms the [stable equilibrium](../../../../../../stable-equilibrium.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
