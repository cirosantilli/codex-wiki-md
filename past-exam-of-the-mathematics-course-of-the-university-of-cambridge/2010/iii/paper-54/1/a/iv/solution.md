<h1 id="1/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $f=1-2M/r$ in the [Schwarzschild metric](../../../../../../../schwarzschild-spacetime.md). For the stationary [Killing vector field](../../../../../../../killing-vector-field.md) $V=\partial_t$, its dual is $V^\flat=-f\,dt$ and the [Papapetrou electromagnetic field](../../../../../../../papapetrou-electromagnetic-field.md) is

$$
F=-f'\,dr\wedge dt=\frac{2M}{r^2}\,dt\wedge dr.
$$

Outside the [Schwarzschild event horizon](../../../../../../../schwarzschild-event-horizon.md), use the static [orthonormal coframe](../../../../../../../orthonormal-coframe-in-spacetime.md) $e^{\hat0}=\sqrt f\,dt$, $e^{\hat r}=dr/\sqrt f$, $e^{\hat\theta}=r\,d\theta$, $e^{\hat\phi}=r\sin\theta\,d\phi$. Then $F=(2M/r^2)e^{\hat0}\wedge e^{\hat r}$. With the [electric field](../../../../../../../electric-field.md) convention $E_{\hat i}=F_{\hat i\hat0}$ from the preceding part,

$$
\boxed{E_{\hat r}=-\frac{2M}{r^2},\qquad \mathbf B=0.}
$$

Thus the stationary [Killing vector field](../../../../../../../killing-vector-field.md) gives a **Coulomb electric field**, directed inward in this convention. If the charge is normalized by $E_{\hat r}=Q/r^2$, its charge is $Q=-2M$. A convention with $F\mapsto-F$ reverses that charge; the invariant content is a radial monopole [electric field](../../../../../../../electric-field.md) of magnitude $2M/r^2$.

For the axial [Killing vector field](../../../../../../../killing-vector-field.md) $V=\partial_\phi$, $V^\flat=r^2\sin^2\theta\,d\phi$, giving

$$
F=2r\sin^2\theta\,dr\wedge d\phi+2r^2\sin\theta\cos\theta\,d\theta\wedge d\phi.
$$

In the same static [orthonormal coframe](../../../../../../../orthonormal-coframe-in-spacetime.md), this is a purely [magnetic field](../../../../../../../magnetic-field.md) with

$$
\boxed{B_{\hat r}=2\cos\theta,\qquad B_{\hat\theta}=-2\sqrt f\sin\theta,\qquad B_{\hat\phi}=0.}
$$

At large $r$ these are the spherical components of $2\mathbf e_z$. This is therefore the **regular magnetic test field asymptotic to a uniform axial field**, distorted by the [Schwarzschild black hole](../../../../../../../schwarzschild-spacetime.md). Its net magnetic monopole flux is zero because the integral of $\cos\theta$ over a sphere vanishes. Both [electromagnetic fields](../../../../../../../electromagnetic-field.md) are regular at the future [event horizon](../../../../../../../event-horizon.md): in [Ingoing Eddington-Finkelstein coordinates](../../../../../../../ingoing-eddington-finkelstein-coordinates.md), the electric field is $(2M/r^2)dv\wedge dr$, and the magnetic two-form already contains only regular spatial coordinates. Static observers themselves cease to exist on the [event horizon](../../../../../../../event-horizon.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 54](../../../../paper-54-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
