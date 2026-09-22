<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**No: the round sphere supplies a counterexample.** On the unit round $S^2\subset\mathbb R^3$, restrict the smooth one-form

$$
\theta=x_3^2\,dx_1.
$$

The [antipodal map](../../../../../../antipodal-map.md) $A(x)=-x$ satisfies $A^*\theta=-\theta$, since $x_3^2$ is unchanged and $dx_1$ changes sign. Every unit-speed closed [geodesic](../../../../../../geodesic.md) is a great circle, with $\gamma(t+\pi)=A(\gamma(t))$. Therefore its two half-circle integrals cancel:

$$
\int_0^{2\pi}\theta_{\gamma(t)}(\dot\gamma(t))\,dt
=\int_0^\pi\bigl(\theta+A^*\theta\bigr)_{\gamma(t)}(\dot\gamma(t))\,dt=0.
$$

The same holds for all repeated traversals and either orientation.

However, its [exterior derivative](../../../../../../exterior-derivative.md) is

$$
d\theta=2x_3\,dx_3\wedge dx_1,
$$

which is not zero on the sphere. For example, at $p=(0,1/\sqrt2,1/\sqrt2)$ the tangent vectors $u=(1,0,0)$ and $w=(0,1/\sqrt2,-1/\sqrt2)$ give $d\theta_p(u,w)=1$. Hence $\theta$ is not a [closed differential form](../../../../../../closed-differential-form.md), and cannot be an [exact differential form](../../../../../../exact-differential-form.md), because $d(dh)=0$. This is the [counterexample to geodesic one-form injectivity on the round sphere](../../../../../../counterexample-to-geodesic-one-form-injectivity-on-the-round-sphere.md); periodic geodesic integrals alone do not imply exactness without an additional geometric hypothesis.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
