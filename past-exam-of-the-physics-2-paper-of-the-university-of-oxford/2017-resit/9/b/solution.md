<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [paraxial approximation](../../../../paraxial-approximation.md) restricts [light rays](../../../../light-ray.md) to small slopes relative to the [optical axis](../../../../optical-axis.md), so $\sin\beta\simeq\tan\beta\simeq\beta$ and geometric lengths can be expanded to second order in height. Treat the source's [optical lens](../../../../lens-optics.md) as a [thin lens](../../../../thin-lens.md) located at $x=0$, with $|y|\ll u,|v|$ and small surface slopes.

For positive real conjugate distances $u,v$, the collapsed-plane geometric path has length

$$
S(y)=\sqrt{u^2+y^2}+\sqrt{v^2+y^2}
\simeq u+v+\frac{y^2}{2}\left(\frac1u+\frac1v\right).
$$

To thin-element accuracy, a segment $s(y)=s_0-\alpha y^2$ of this path lies inside the [optical lens](../../../../lens-optics.md), replacing the same length of air. The geometric air path is $S-s$, the material path is $s$, and the [optical path length](../../../../optical-path-length.md) and travel time are therefore

$$
\mathcal L(y)=S(y)+(n-1)s(y),\qquad
ct(y)\simeq u+v+(n-1)s_0
+y^2\left[\frac1{2u}+\frac1{2v}-(n-1)\alpha\right].
$$

This distinguishes geometric length from [optical path length](../../../../optical-path-length.md); adding $ns$ to $S$ without subtracting the replaced air would count that segment twice.

For a nonaxial [light ray](../../../../light-ray.md), [Fermat's principle](../../../../fermat-principle.md) gives $d\mathcal L/dy=0$ and hence

$$
\frac1u+\frac1v=2(n-1)\alpha.
$$

The [focal length](../../../../focal-length.md) is obtained with the incident object at infinity:

$$
\boxed{\frac1f=2(n-1)\alpha,\qquad f=\frac1{2(n-1)\alpha}.}
$$

The constant thickness $s_0$ supplies a common delay but does not change the leading [focal length](../../../../focal-length.md). Since $\alpha$ has units of inverse [length](../../../../length.md), this formula has the correct dimensions. These are [thin lens](../../../../thin-lens.md) results; [paraxial approximation](../../../../paraxial-approximation.md) alone does not remove finite-thickness corrections in a general [thick lens](../../../../thick-lens.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
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
