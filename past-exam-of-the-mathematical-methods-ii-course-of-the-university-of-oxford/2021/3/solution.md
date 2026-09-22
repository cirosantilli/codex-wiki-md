<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [arc length](../../../arc-length.md) of the [helix](../../../helix.md) follows from its parametrization:

$$
\mathbf r'(t)=\bigl(-10\sin(t-\pi/2),\ 10\cos(t-\pi/2),\ 5\bigr),\qquad
|\mathbf r'(t)|=\sqrt{100+25}=5\sqrt5.
$$

Thus $\ell_h=15\pi\sqrt5\,\mathrm m$. Its endpoint is $(0,20,15\pi)$, at height $h=15\pi\,\mathrm m$.

Under the usual intended interpretation that the descending quarter of a [circle](../../../circle.md) drops through one [radius](../../../radius.md), its [radius](../../../radius.md) is $R=h$. Its [arc length](../../../arc-length.md) is $\ell_c=\pi R/2=15\pi^2/2\,\mathrm m$, giving

$$
\boxed{\ell_h+\ell_c=15\pi\sqrt5+\frac{15\pi^2}{2}=179.39425397\ldots\,\mathrm m\simeq179\,\mathrm m.}
$$

**The printed smoothness condition is inconsistent.** The terminal [tangent vector](../../../tangent-vector-split.md) of the [helix](../../../helix.md) is $\mathbf r'(3\pi)=(-10,0,5)$. Every [tangent vector](../../../tangent-vector-split.md) to a [curve](../../../curve.md) confined to the $yz$ [plane](../../../plane.md) has zero $x$ component, so no such [regular curve](../../../regular-curve.md) can join this [helix](../../../helix.md) with a common [tangent line](../../../tangent-line.md). Moreover, the [helix](../../../helix.md) is still rising at that endpoint. Thus no smooth ride satisfying all the literal conditions exists.

Even after allowing a corner, a quarter of a [circle](../../../circle.md) reaching the ground does not alone determine its [radius](../../../radius.md): the orientation of its endpoint radii must also be specified. For example, in the $yz$ [plane](../../../plane.md), the circular arc

$$
y=20+R\bigl(\cos\theta-\cos\theta_0\bigr),\quad
z=h+R\bigl(\sin\theta-\sin\theta_0\bigr),\quad
\theta_0-\pi/2\le\theta\le\theta_0,
$$

traversed toward decreasing $\theta$, descends monotonically for $0\le\theta_0\le\pi/2$ and reaches $z=0$ when $R=h/(\sin\theta_0+\cos\theta_0)$. Choosing $\theta_0=\pi/4$ gives $R=h/\sqrt2$, whereas $\theta_0=\pi/2$ gives $R=h$. The numerical answer above is conditional on the intended $R=h$ geometry; it does not repair the impossible smooth join.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2021](../../2021-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
